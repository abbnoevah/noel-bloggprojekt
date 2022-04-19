<template>
  <div>
    <div>
      <div>
        <div
          class="bg-fixed w-full sm:w-full h-screen bg-cover bg-top"
          style="background-image: url(/images/big-sur-mountains-clear-sky-sunrise-dawn-morning-macos-big-5120x2880-1496.jpg);"
        >
          <div
            class="bg-black bg-opacity-40 w-full h-full flex flex-col items-center"
          >
            <div
              class="flex flex-col md:flex-row justify-center mt-64 md:mt-96 min-w-10/12 md:w-11/12 gap-12"
            >
              <div
                class="text-white md:pl-40 text-5xl md:text-8xl w-full md:w-1/2 text-center md:text-left"
                style="text-shadow: 0 0 16px rgba(0, 0, 30, 0.6)"
              >
                <p>Visit<br />California</p>
              </div>

              <div
                class="text-white md:pr-40 md:w-1/2 w-full flex flex-col justify-center md:items-end text-center"
              >
                <div
                  class="text-lg md:text-2xl w-full"
                  style="text-shadow: 0 0 16px rgba(0, 0, 30, 0.6)"
                >
                  <p class="font-light w-full md:text-right">Blog by</p>
                </div>
                <div
                  class="w-full text-2xl  md:text-5xl"
                  style="text-shadow: 0 0 16px rgba(0, 0, 30, 0.6)"
                >
                  <p class="w-full md:text-right font-light">
                    <nuxt-link to="/contacts">Noel Vahlström</nuxt-link>
                  </p>
                </div>
              </div>
            </div>

            <div
              class="w-full h-96"
              style="background: rgb(17, 24, 39); background: linear-gradient(0deg, rgba(17, 24, 39, 1) 0%, rgba(17, 24, 39, 0.8) 25%, rgba(17, 24, 39, 0.6) 50%,rgba(252, 255, 255, 0) 100%);"
            ></div>
          </div>
        </div>
      </div>

      <div
        class="bg-gray-900 min-w-full min-h-screen py-32 flex flex-col items-center justify-center"
      >
        <div class="h-full w-full">
          <!-- TITLE -->
          <div
            class="w-full h-20 flex justify-center flex-row text-2xl md:text-5xl gap-8 pb-4 font-light bg-cover"
          >
            <p class="h-full text-white">POPULAR</p>
            <p class="h-full" style="color: rgba(255, 136, 80, 1)">LOCATIONS</p>
          </div>

          <!-- LINE -->
          <div class="opacity-70">
            <hr
              class="w-full mb-8"
              style="border: none; height: 2px; background: rgb(255, 136, 80); background: linear-gradient(90deg, rgba(255, 136, 80, 0) 0%, rgba(255, 136, 80, 0.7) 25%, rgba(255, 136, 80, 1) 50%, rgba(255, 136, 80, 0.7) 75%, rgba(255, 136, 80, 0) 100%);"
            />
          </div>

          <!-- CARDS -->
          <div
            class="py-8 mt-16"
            style="background: rgb(28, 49, 79); background: linear-gradient(90deg, rgba(28, 49, 79, 0) 0%, rgba(24, 41, 66, 1) 100%);"
          >
            <div
              class="flex flex-col md:flex-row sm:h-24 md:h-96 md:w-full sm:w-3/4 items-center md:justify-center gap-8 md:gap-32 bg-opacity-60" style="perspective: 800px;"
            >

            <PostComponent v-for="item in list1" :key="item.id" :item="item"/>

              <!-- <li style="transform: rotatey(15deg);">
                <nuxt-link to="/losAng">
                  <div
                    class="md:h-80 w-80 md:w-96 z-99 bg-cover shadow-2xl text-center text-white text-2xl md:text-4xl rounded-xl md:rounded-2xl"
                    style="
                      background-image: url(/images/551763.jpg);
                      text-shadow: 0 0 12px rgba(0, 0, 30, 1);
                    "
                  >
                    <h1
                      class="h-full w-full bg-black bg-opacity-30 hover:bg-black hover:bg-opacity-0 p-8 rounded-xl md:rounded-2xl"
                    >
                      Los Angeles
                    </h1>
                  </div>
                </nuxt-link>
              </li> -->

              <!-- <li style="transform: rotatey(8deg);">
                <nuxt-link to="/lasVeg">
                  <div
                    class="md:h-72 w-80 md:w-96 z-99 bg-cover shadow-2xl text-center text-white text-2xl md:text-4xl rounded-xl md:rounded-2xl"
                    style="
                      background-image: url(/images/las-vegas-movies-2048x1242.jpg);
                      text-shadow: 0 0 12px rgba(0, 0, 30, 1);
                    "
                  >
                    <h1
                      class="h-full w-full bg-black bg-opacity-30 hover:bg-black hover:bg-opacity-0 p-8 rounded-xl md:rounded-2xl"
                    >
                      Las Vegas
                    </h1>
                  </div>
                </nuxt-link>
              </li> -->

              <!-- <li style="transform: rotatey(6deg);">
                <nuxt-link to="/sanFran">
                  <div
                    class="md:h-64 w-80 md:w-96 z-99 bg-cover shadow-2xl text-center text-white text-2xl md:text-4xl rounded-xl md:rounded-2xl"
                    style="
                      background-image: url(/images/685669.jpg);
                      text-shadow: 0 0 12px rgba(0, 0, 30, 1);
                    "
                  >
                    <h1
                      class="h-full w-full bg-black bg-opacity-30 hover:bg-black hover:bg-opacity-0 p-8 rounded-xl md:rounded-2xl"
                    >
                      San Francisco
                    </h1>
                  </div>
                </nuxt-link>
              </li> -->
            </div>
          </div>

          <div
            class="md:w-full h-16 shadow-2xl hidden md:flex mb-40"
            style="background: rgb(0, 0, 0); background: linear-gradient(90deg, rgba(0, 0, 0, 0) 0%, rgba(255, 136, 80, 1) 20%,rgba(0, 0, 0, 0) 100%);margin-top: -200px;"
          ></div>

          <!-- TITLE -->
          <div
            class="w-full h-20 flex justify-center flex-row text-2xl md:text-5xl gap-8 mt-46 pt-32 pb-20 font-light "
          >
            <p class="h-full text-white">OTHER</p>
            <p class="h-full" style="color: rgba(255, 136, 80, 1)">LOCATIONS</p>
          </div>

          <!-- LINE -->
          <div class="opacity-70">
            <hr
              class="w-full mb-8"
              style="border: none; height: 2px; background: rgb(255, 136, 80); background: linear-gradient(90deg, rgba(255, 136, 80, 0) 0%, rgba(255, 136, 80, 0.7) 25%, rgba(255, 136, 80, 1) 50%, rgba(255, 136, 80, 0.7) 75%, rgba(255, 136, 80, 0) 100%);"
            />
          </div>

          <!-- CARDS -->
          <div
            class="py-8 mt-16"
            style="background: rgb(28, 49, 79); background: linear-gradient(90deg, rgba(24, 41, 66, 1) 0%, rgba(28, 49, 79, 0) 100%);"
          >
            <div
              class="flex flex-col md:flex-row sm:h-24 md:h-96 md:w-full sm:w-3/4 items-center md:justify-center gap-8 md:gap-32 bg-opacity-60" style="perspective: 800px;"
            >
              <PostComponent v-for="item in list2" :key="item.id" :item="item"/>
              <!-- <li style="transform: rotatey(-6deg);">
                <nuxt-link to="/yosemite">
                  <div
                    class="md:h-64 w-80 md:w-96 bg-cover shadow-2xl text-center text-white text-2xl md:text-4xl rounded-xl md:rounded-2xl"
                    style="
                      background-image: url(/images/yosemite2.jpg);
                      text-shadow: 0 0 12px rgba(0, 0, 30, 1);
                    "
                  >
                    <h1
                      class="h-full w-full bg-black bg-opacity-30 hover:bg-black hover:bg-opacity-0 p-8 rounded-xl md:rounded-2xl"
                    >
                      Yosemite
                    </h1>
                  </div>
                </nuxt-link>
              </li> -->

              <!-- <li style="transform: rotatey(-8deg);">
                <nuxt-link to="/carmel">
                  <div
                    class="md:h-72 w-80 md:w-96 bg-cover shadow-2xl text-center text-white text-2xl md:text-4xl rounded-xl md:rounded-2xl"
                    style="
                      background-image: url(/images/carmel.jpg);
                      text-shadow: 0 0 12px rgba(0, 0, 30, 1);
                    "
                  >
                    <h1
                      class="h-full w-full bg-black bg-opacity-30 hover:bg-black hover:bg-opacity-0 p-8 rounded-xl md:rounded-2xl"
                    >
                      Carmel by the Sea
                    </h1>
                  </div>
                </nuxt-link>
              </li> -->

              <!-- <li style="transform: rotatey(-15deg);">
              <div class="h-full w-full">
                
              </div>
                <nuxt-link to="/sacramento">
                  <div
                    class="md:h-80 w-80 md:w-96 bg-cover shadow-2xl text-center text-white text-2xl md:text-4xl rounded-xl md:rounded-2xl"
                    style="
                      background-image: url(/images/sacramento.jpg);
                      text-shadow: 0 0 12px rgba(0, 0, 30, 1);
                    "
                  >
                    <h1
                      class="h-full w-full bg-black bg-opacity-30 hover:bg-black hover:bg-opacity-0 p-8 rounded-xl md:rounded-2xl"
                    >
                      Sacramento
                    </h1>
                  </div>
                </nuxt-link>
              </li> -->
            </div>
          </div>

          <div
            class="md:w-full h-16 shadow-2xl hidden md:flex mb-40"
            style="
              background: rgb(0, 0, 0); background: linear-gradient(90deg, rgba(0, 0, 0, 0) 0%, rgba(255, 136, 80, 1) 80%, rgba(0, 0, 0, 0) 100%); margin-top: -200px;"
          >
          </div>
        </div>
      </div>

      <div class="flex flex-col">
        <div
          class="w-full h-screen pb-96 shadow-2xl shadow-black flex flex-row flex-wrap justify-center bg-cover bg-top"
          style="background-image: url(/images/3181241.jpg)"
        >
          <div
            class="w-full h-screen"
            style="
              background: rgb(17, 24, 39); background: linear-gradient(180deg, rgba(17, 24, 39, 1) 0%, rgba(17, 24, 39, 0.8) 25%, rgba(17, 24, 39, 0.6) 50%, rgba(0, 0, 0, 0) 100%);">
            <div
              class="h-full w-full flex flex-col justify-center items-center text-white"
            >
              <div class="h-full w-5/6 md:w-8/12 text-center bg-black bg-opacity-0 p-8 md:p-24">
                <p class="text-3xl md:text-6xl font-light">MIN RESA</p>

                <nuxt-content :document="blog_Resa" class="text-white w-full h-full"></nuxt-content>
              </div>
            </div>
          </div>

          <!-- <div class="min-h-screen w-full bg-black bg-opacity-40" ></div> -->
        </div>
      </div>
    </div>

  <credits class="relative" style="box-shadow: 0 0 32px 0 rgba(0,0,0,0.4);"/>

  </div>
</template>

<script>

import PostComponent from "../components/PostComponent.vue";

export default {
  name: "IndexPage",

  async asyncData({ $content }) {
    let blog_Resa = await $content("minResa").without(['body']).fetch();
    const list1 = await $content("locations").sortBy('id', 'asc').limit(3).without(['body']).fetch();
    const list2 = await $content("locations").sortBy('id', 'asc').skip(3).limit(3).without(['body']).fetch();

    console.log(list1);

    // resa = resa.filter(function (page) {
    //   console.log(page.theme);
    //   if (page.title === "Min Resa") return true;
    //   return false;
    // });

    return {
      blog_Resa,
      list1,
      list2
    };
  },

  data() {
        return {
            PostComponent
        }
    },

  methods: {
    goToDish(id) {
      this.$router.push('/posts/'+id)
    }
  }
};
</script>

<style></style>

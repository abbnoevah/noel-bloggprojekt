<template>
<div>
    <div class="min-h-screen w-full bg-cover flex justify-center text-white text-2xl md:text-6xl" style="background-image: url(/images/big-sur-mountains-clear-sky-sunrise-dawn-morning-macos-big-5120x2880-1496.jpg);">
        <div class="w-11/12 md:w-10/12 my-40 md:m-16">
            <ul class="w-full h-fullflex flex-col">
                <li class="w-full h-full gap-8">
                    <PostComponent class="flex flex-row h-1/2 w-1/3" v-for="item in list1" :key="item.id" :item="item" id="placeList1"/>
                    <PostComponent class="flex flex-row h-1/2 w-1/3" v-for="item in list2" :key="item.id" :item="item" id="placeList2"/>
                </li>
            </ul>
        </div>
    </div>

    <credits />
</div>
</template>

<script>

import PostComponent from "../components/PostComponent.vue";

export default {

    async asyncData({ $content }) {
    let blog_Resa = await $content("minResa").fetch();
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
        
    }

    
}





</script>
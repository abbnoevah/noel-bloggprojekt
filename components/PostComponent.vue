<template>
<nuxt-link :to="`/posts/${item.id}`">
    <div>
        <div
        class="md:h-80 w-80 md:w-96 bg-cover shadow-2xl text-center text-white text-2xl md:text-4xl rounded-xl md:rounded-2xl"
        :style="{
          backgroundImage: `url(${item.image})`,
          textShadow: '0 0 12px rgba(0, 0, 30, 1)'
          }">
            <h1
            class="h-full w-full bg-black bg-opacity-30 hover:bg-black hover:bg-opacity-40 hover:text-gray-300 p-8 rounded-xl md:rounded-2xl"
            >
            {{item.title}}
            </h1>
        </div>
    </div>
</nuxt-link>
</template>

<script>
export default {
  props: ["item"],

  data() {
    return {};
  },
};
</script>
<template>
<div class="w-full mx-auto" :style="{
          backgroundImage: `url(${item.image})`,
          }">>
    <!-- <img :src="city.image" />
    <h1 class="text-5xl mb-8">{{city.title}}</h1>
    <p class="mb-8">{{city.description}}</p>
    <nuxt-content :document="city"></nuxt-content> -->
</div>
</template>
<script>
export default {
    async asyncData({$content, params}) {
        const list1 = await $content("locations").sortBy('id', 'asc').limit(3).without(['body']).fetch();
        const list2 = await $content("locations").sortBy('id', 'asc').skip(3).limit(3).without(['body']).fetch();
        let city = await $content('locations/location'+params.id).fetch()
        console.log(city)
        return {
            city,
            list1,
            list2
        }
    },
}
</script>
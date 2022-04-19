<template>
<div class="w-full min-h-screen mx-auto bg-gray-800 bg-cover" :style="{ backgroundImage: `url(${city.image})`}">
    <div class="w-full min-h-screen bg-black bg-opacity-50 flex justify-center">
        <div class="pt-40 w-5/6 h-full text-white text-center">
            <h1 class="text-5xl mb-8">{{city.title}}</h1>
            <p class="mb-8">{{city.description}}</p>
            <nuxt-content :document="city" ></nuxt-content>
        </div>
    </div>
    <credits class="relative" style="box-shadow: 0 0 32px 0 rgba(0,0,0,0.4);"/>
</div>
</template>
<script>


export default {

    props: ["item"],
    
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
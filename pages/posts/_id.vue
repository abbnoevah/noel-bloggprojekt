<template>
<div class="w-full min-h-screen mx-auto bg-gray-800 bg-cover bg-fixed" :style="{ backgroundImage: `url(${city.image})`}">
    <div class="w-full min-h-screen bg-black bg-opacity-40 flex items-center flex-col">
        <div class="md:p-16 w-5/6 md:w-1/2 text-white text-center m-40">
            <h1 class="text-6xl mb-8" style="text-shadow: 0 0 16px rgba(0, 0, 30, 1)">{{city.title}}</h1>
            <!-- <p class="mb-8">{{city.description}}</p> -->
            <div class="opacity-70">
                <hr
                class="w-full mt-12"
                style="border: none; height: 2px; background: rgb(180, 180, 230); background: linear-gradient(90deg, rgba(180, 180, 230, 0) 0%, rgba(180, 180, 230, 0.7) 25%, rgba(180, 180, 230, 1) 50%, rgba(180, 180, 230, 0.7) 75%, rgba(180, 180, 230, 0) 100%);"
                />
            </div>
            <nuxt-content :document="city" class="text-lg md:text-xl pt-8 pb-0 text-justify" style="text-shadow: 0 0 8px rgba(0, 0, 30, 1)"></nuxt-content>
            <hr
                class="w-full mt-12"
                style="border: none; height: 2px; background: rgb(180, 180, 230); background: linear-gradient(90deg, rgba(180, 180, 230, 0) 0%, rgba(180, 180, 230, 0.7) 25%, rgba(180, 180, 230, 1) 50%, rgba(180, 180, 230, 0.7) 75%, rgba(180, 180, 230, 0) 100%);"
                />
            <div class="w-full h-48 md:h-96 bg-cover mt-12 border-2 border-white" :style="{backgroundImage: `url(${city.image2})` }" style="box-shadow: 0 16px 32px 0 rgba(0,0,0,0.4);"></div>
        </div>
        <!-- <div class="h-16 w-40 bg-gray-800" @click="city.id"></div> -->
        
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

        return {
            city,
            list1,
            list2
        }
    },
}
</script>
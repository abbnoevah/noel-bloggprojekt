<template>

<div>
    <div class="w-full flex justify-center" style="box-shadow: 0 0 32px 0 rgba(0,0,0,1);">
        <div class="w-full md:w-full flex flex-row-reverse md:flex-row flex-wrap">
            <div class="w-1/2 md:w-1/4 h-80 bg-gray-900">
            </div>
                <div class="w-1/2 md:w-1/4 h-80 flex flex-col bg-gray-900">
                    <ul class="w-full h-full text-gray-400 p-8 font-mono" style="text-shadow: 0 0 8px rgba(0, 0, 30, 1);">
                        <li class="w-full h-1/6 flex items-center justify-center text-center hover:text-gray-200 md:text-xl" id="LA"><nuxt-link to="/posts/1">Los Angeles</nuxt-link></li>
                        <li class="w-full h-1/6 flex items-center justify-center text-center hover:text-gray-200 md:text-xl" id="LV"><nuxt-link to="/posts/2">Las Vegas</nuxt-link></li>
                        <li class="w-full h-1/6 flex items-center justify-center text-center hover:text-gray-200 md:text-xl" id="SF"><nuxt-link to="/posts/3">San Francisco</nuxt-link></li>
                        <li class="w-full h-1/6 flex items-center justify-center text-center hover:text-gray-200 md:text-xl" id="YM"><nuxt-link to="/posts/4">Yosemite</nuxt-link></li>
                        <li class="w-full h-1/6 flex items-center justify-center text-center hover:text-gray-200 md:text-xl" id="CA"><nuxt-link to="/posts/5">Carmel by the Sea</nuxt-link></li>
                        <li class="w-full h-1/6 flex items-center justify-center text-center hover:text-gray-200 md:text-xl" id="SM"><nuxt-link to="/posts/6">Sacramento</nuxt-link></li>
                    </ul>
                </div>
                <div class="w-1/2 md:w-1/4 h-80 bg-gray-900">
                    <ul class="w-full h-full text-gray-400 flex flex-col " style="text-shadow: 0 0 16px rgba(0, 0, 30, 1);">
                        <li class="w-full h-1/2 flex items-center justify-center text-center md:text-4xl hover:bg-white hover:bg-opacity-0 hover:text-gray-200" id="abtBtn"><nuxt-link to="/about-me">About Me</nuxt-link></li>
                        <li class="w-full h-1/2 flex items-center justify-center text-center md:text-4xl hover:bg-white hover:bg-opacity-0 hover:text-gray-200" id="ctcBtn"><nuxt-link to="/contacts">Contact</nuxt-link></li>
                    </ul>
                </div>
            <div class="w-1/2 md:w-1/4 h-80 bg-gray-900"></div>
            <div class="w-full h-20 flex flex-row justify-center items-center text-gray-400 bg-gray-800 " style="box-shadow: 0 0 32px 0 rgba(0,15,30,0.6); text-shadow: 0 0 8px rgba(0, 0, 30, 1);">
                <a class="text-2xl hover:text-gray-200" id="desInsp" href="https://mir-s3-cdn-cf.behance.net/project_modules/source/c31f26102204477.5f316a3b27b41.jpg">Design Inspiration</a>
            </div>
        </div>
    </div>
</div>

</template>

<style>

#ctcBtn:hover {
    transition: 200ms;
    border-radius: 16px;
}

#abtBtn:hover {
    transition: 200ms;
    border-radius: 16px;
}
</style>
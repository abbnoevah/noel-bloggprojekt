<template>

<div>
    <div class="w-full bg-gray-900 flex justify-center" style="box-shadow: 0 0 32px 0 rgba(0,0,0,1);">
        <div class="w-full md:w-5/6 flex flex-row-reverse md:flex-row flex-wrap">
            <div class="w-1/2 md:w-1/4 h-96">
            </div>
            <div class="w-1/2 md:w-1/4 h-96 flex flex-col">
                <ul class="w-full h-3/4 text-gray-400 p-8 font-mono" style="text-shadow: 0 0 8px rgba(0, 0, 30, 1);">
                    <li class="w-full h-1/6 flex items-center hover:text-gray-200"><nuxt-link to="/losAng">Los Angeles</nuxt-link></li>
                    <li class="w-full h-1/6 flex items-center hover:text-gray-200"><nuxt-link to="/lasVeg">Las Vegas</nuxt-link></li>
                    <li class="w-full h-1/6 flex items-center hover:text-gray-200"><nuxt-link to="/sanFran">San Francisco</nuxt-link></li>
                    <li class="w-full h-1/6 flex items-center hover:text-gray-200"><nuxt-link to="/yosemite">Yosemite</nuxt-link></li>
                    <li class="w-full h-1/6 flex items-center hover:text-gray-200"><nuxt-link to="/carmel">Carmel by the Sea</nuxt-link></li>
                    <li class="w-full h-1/6 flex items-center hover:text-gray-200"><nuxt-link to="/sacramento">Sacramento</nuxt-link></li>
                </ul>
            </div>
            <div class="w-1/2 md:w-1/4 h-96">
                <ul class="w-full h-3/4 text-gray-400 flex flex-col " style="text-shadow: 0 0 16px rgba(0, 0, 30, 1);">
                    <li class="w-full h-1/2 flex items-center justify-center text-center md:text-4xl hover:bg-white hover:bg-opacity-10 hover:text-gray-200"><nuxt-link to="/about-me">About Me</nuxt-link></li>
                    <li class="w-full h-1/2 flex items-center justify-center text-center md:text-4xl hover:bg-white hover:bg-opacity-10 hover:text-gray-200"><nuxt-link to="/contacs">Contact</nuxt-link></li>
                </ul>
            </div>
            <div class="w-1/2 md:w-1/4 h-96"></div>
        </div>
    </div>
</div>

</template>
<template>

<div>
    <div class="min-h-screen w-full bg-cover flex justify-center text-white text-6xl" style="background-image: url(/images/big-sur-mountains-clear-sky-sunrise-dawn-morning-macos-big-5120x2880-1496.jpg);">
        <div class="w-1/2 m-40">
            <ul class="w-full flex flex-col gap-16">
                <li id="yt" class="h-48 w-full rounded-2xl" style="box-shadow: 0 0 32px 0 rgba(0,0,0,0.4); background: rgb(190,72,72); background: radial-gradient(circle, rgba(190,72,72,1) 0%, rgba(55,31,34,0.85) 80%, rgba(39,17,22,0.7) 100%); text-shadow: 0 0 8px rgba(0, 0, 30, 0.8);">
                    <a href="https://www.youtube.com/channel/UCVHONdKTEQv9DPkPJFRdGZA" target="blank" class="w-full h-full bg-black bg-opacity-10 flex justify-center items-center">
                        <h1>Youtube</h1>
                    </a>
                </li>
                <li id="ig" class="h-48 w-full rounded-2xl" style="box-shadow: 0 0 32px 0 rgba(0,0,0,0.4); background: rgb(173,73,98); background: radial-gradient(circle, rgba(173,73,98,1) 0%, rgba(55,31,41,0.85) 80%, rgba(39,17,34,0.7) 100%); text-shadow: 0 0 8px rgba(0, 0, 30, 0.8);">
                    <a href="https://www.instagram.com/irsta.noel/" target="blank" class="w-full h-full bg-black bg-opacity-10 flex justify-center items-center">
                        <h1>Instagram</h1>
                    </a>
                </li>
                <li id="fb" class="h-48 w-full rounded-2xl" style="box-shadow: 0 0 32px 0 rgba(0,0,0,0.4); background: rgb(73,100,173); background: radial-gradient(circle, rgba(73,98,173,1) 0%, rgba(31,41,55,0.85) 80%, rgba(17,24,39,0.7) 100%); text-shadow: 0 0 8px rgba(0, 0, 30, 0.8);">
                    <a href="https://www.youtube.com/watch?v=pwTzHbIXSlI" target="blank" class="w-full h-full bg-black bg-opacity-10 flex justify-center items-center">
                        <h1>Facebook</h1>
                    </a>
                </li>
            </ul>
        </div>
    </div>

    <credits class="relative" style="box-shadow: 0 0 32px 0 rgba(0,15,25,0.4);"/>
</div>

</template>

<style>

#yt:hover {
    transform: scale(0.96);
    transition: 150ms;
}
#ig:hover {
    transform: scale(0.96);
    transition: 150ms;
}
#fb:hover {
    transform: scale(0.96);
    transition: 150ms;
}

</style>
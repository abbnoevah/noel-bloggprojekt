<template>

<div>
    <div class="min-h-screen w-full bg-cover flex justify-center text-white text-2xl md:text-6xl" style="background-image: url(/images/big-sur-mountains-clear-sky-sunrise-dawn-morning-macos-big-5120x2880-1496.jpg);">
        <div class="w-3/4 md:w-1/2 my-40 md:m-40">
            <ul class="w-full flex flex-col gap-16">
                <li id="yt" class="h-48 w-full rounded-2xl" style="box-shadow: 0 12px 32px 0 rgba(0,0,0,0.8); background: rgb(18,4,48); background: linear-gradient(20deg, rgba(18,4,48,1) 0%, rgba(129,26,26,1) 100%);">
                    <a href="https://www.youtube.com/channel/UCVHONdKTEQv9DPkPJFRdGZA" target="blank" class="w-full h-full bg-black bg-opacity-10 flex justify-center items-center">
                        <h1>Youtube</h1>
                    </a>
                </li>
                <li id="ig" class="h-48 w-full rounded-2xl" style="box-shadow: 0 12px 32px 0 rgba(0,0,0,0.8); background: rgb(173,73,98); background: rgb(18,4,48); background: linear-gradient(20deg, rgba(18,4,48,1) 0%, rgba(117,27,53,1) 100%);">
                    <a href="https://www.instagram.com/irsta.noel/" target="blank" class="w-full h-full bg-black bg-opacity-10 flex justify-center items-center">
                        <h1>Instagram</h1>
                    </a>
                </li>
                <li id="fb" class="h-48 w-full rounded-2xl" style="box-shadow: 0 12px 32px 0 rgba(0,0,0,0.8); background: rgb(18,4,48); background: linear-gradient(20deg, rgba(18,4,48,1) 0%, rgba(26,92,129,1) 100%);">
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
<template>
    <div class="flex flex-col justify-between relative h-[68vh] w-[90vw]
    items-center bg-gradient-to-r from-[#370665] to-[#35589A] rounded-[1.8rem]">
        <img src="/imgSrc/qr.png" class="scale-[0.4] absolute origin-top mt-10">

        <h1 id="scan">Scan QR code for more</h1>
        <h1 id="download">Now you can download the official musify app.</h1>

        <img src="/imgSrc/googlePlay.png" class="scale-[0.5] hover:scale-[0.55] active:scale-50 cursor-pointer">
        <img src="/imgSrc/appStore.png" class="scale-[0.5] -mt-20 hover:scale-[0.55] active:scale-50 cursor-pointer">
    </div>
</template>

<script>
export default {
    
}
</script>

<style>
#scan{
    font-family: proximaBold;
    @apply text-white text-3xl mt-52 text-center w-[95%]
}
#download{
    @apply text-white text-2xl mb-auto text-center w-[95%]
}
</style>
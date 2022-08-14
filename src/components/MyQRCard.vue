<template>
    <div class="flex flex-col justify-between relative h-[72vh] w-[70vw]
    items-center bg-gradient-to-r from-[#370665] to-[#35589A] rounded-[1.8rem]
    md:flex-row md:h-[20rem] md:items-end md:w-[90vw] xl:w-[70vw]">
        <img src="/imgSrc/qr.png" class="scale-[0.4] absolute origin-top mt-10 md:origin-center md:scale-[0.6] md:-ml-10 xl:scale-75 lg:ml-5 lg:origin-center lg:mt-4">

        <div class="flex flex-col justify-between items-center relative md:ml-auto md:mb-10 md:-mr-10">
            <h1 id="scan">Scan QR code for more</h1>
            <h1 id="download">Now you can download the official musify app.</h1>

            <div class="flex flex-col justify-center items-center md:flex-row md:w-[30%]">
                <img src="/imgSrc/googlePlay.png" class="scale-[0.5] md:scale-[0.8] hover:scale-[0.55] active:scale-50 md:hover:scale-[0.85] md:active:scale-[0.8] cursor-pointer">
                <img src="/imgSrc/appStore.png" class="scale-[0.5] md:scale-[0.8] -mt-20 md:-mt-0 hover:scale-[0.55] active:scale-50 md:hover:scale-[0.85] md:active:scale-[0.8] cursor-pointer">
            </div>
        </div>
    </div>
</template>

<script>
export default {
    
}
</script>

<style scoped>
#scan{
    font-family: proximaBold;
    @apply text-white text-3xl mt-52 text-center w-[95%]
}
#download{
    @apply text-white text-2xl mb-auto text-center w-[95%] md:w-[50%]
}
</style>
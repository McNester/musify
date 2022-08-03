<template >
    <div 
    class="flex flex-col justify-start items-center h-[60vh] w-[70%] bg-gradient-to-r from-[#370665] to-[#35589A] rounded-[1.8rem]
    md:w-[95%] md:h-[30vh]">
        <h1 class="text-3xl text-center mt-5">Why buy directly from Musify?</h1>
        <div 
        class="flex flex-col justify-start items-center h-[70%] w-[100%] 
        md:flex-row md:gap-10 my-auto">

            <div 
            class="feature md:ml-10">
                <img src="/imgSrc/delivery.svg">
                <h1 class="md:w-[40%] lg:w-[100%]">Free delivery</h1>
            </div>
            <div 
            class="feature mr-2">
                <img src="/imgSrc/verify.svg">
                <h1 >Verified Products</h1>
            </div>
            <div 
            class="feature mb-auto md:mb-0 md:mr-10">
                <img  src="/imgSrc/support.svg">
                <h1>24/7 Customer support</h1>
            </div>

        </div>


    </div>
</template>

<script>
export default {
    
}
</script>

<style scoped>
h1{
    color: white;
    font-family: proximaBold;
}
.feature{
    @apply flex justify-start mt-auto md:mt-0 items-center gap-5 text-2xl w-[50%] sm:w-[60%] sm:scale-110 md:w-[40%] md:scale-100 lg:scale-[1.2] 
}
</style>
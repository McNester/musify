<template>
    <div class=' 
    cursor-pointer hover:scale-105 active:scale-100 
    flex flex-col justify-end items-center 
    w-[15rem] h-[14rem] relative ml-[0.6rem] rounded-[2rem] transition-all ease-in-out
    md:scale-[1.2] md:hover:scale-[1.3] md:active:scale-[1.2] md:ml-[2.9rem] 
    lg:scale-100 lg:hover:scale-105 lg:active:scale-100 lg:ml-0'>

        <img class="absolute scale-[0.9] top-0 mt-6 z-10" src="/imgSrc/headPhoneRed.png">
        <div 
        class="flex flex-col items-start justify-end w-11/12 h-1/2 
        bg-[#282828] bg-opacity-70 px-2 rounded-[1.2rem]
        shadow-[#000000] shadow-[0px_10px_20px_-10px]
        lg:bg-transparent lg:shadow-none lg:border-white lg:border-[0.001rem] lg:backdrop-blur-sm">
            <h1>
                Wireless Headphones
            </h1>
            <div class="flex w-full justify-start p-2 gap-5">
                <h1 id="cost" class=" text-sm">$120</h1>
                <h1 class=" line-through text-[0.80rem]">$185</h1>
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
    font-family: proxima;
    @apply text-white lg:text-black
}
#cost{
    @apply text-[#FC9918]
}

</style>
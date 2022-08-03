<template >



    <div
    @click.stop
    class="lg:flex justify-between items-center w-2/5 h-ful hidden ml-auto mr-20"
    >
        <h1 @click="$emit('home')">Home</h1>
        <h1 @click="$emit('explore')" >Explore</h1>
        <h1 @click="$emit('contact')">Contact us</h1>
    </div>



</template>
<script>

</script>
<style scoped>
h1{
    font-family: proximaLight;
    @apply text-2xl cursor-pointer transition-all ease-in-out underline-offset-2 decoration-[#F14A16] hover:underline decoration-2 
}
</style>
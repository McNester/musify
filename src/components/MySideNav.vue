<template >

    
    <div
    v-if="isVisible"
    @click="$emit('invisible')"
    class="h-[509rem] w-screen 
    bg-gray-900 bg-opacity-30 absolute top-0 z-10
    ">


        <div
        v-if="isVisible"
        @click.stop
        class=" w-2/5 h-full bg-white"
        >
            <h1 @click="$emit('home')">Home</h1>
            <h1 @click="$emit('explore')" >Explore</h1>
            <h1 @click="$emit('contact')">Contact us</h1>
        </div>
    </div>



</template>
<script>
export default {
    props:{
        isVisible: Boolean
    },
    
    
}
</script>
<style scoped>
h1{
    font-family: proxima;
    @apply p-1 text-xl pl-5 hover:scale-105 cursor-pointer active:scale-100 md:text-4xl
}
</style>
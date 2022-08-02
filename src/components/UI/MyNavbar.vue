<template>

    <div class="flex justify-between items-center h-16 w-screen fixed z-50 bg-white">
        
            <img @click="showSideNav" src="/imgSrc/hamburger.svg" 
            class="hover:scale-[1.2] pl-10 cursor-pointer active:scale-100
            ">
             
            <MySideNav @invisible="this.isSideNavVisible=false" @home="goToHome" @explore="goToExplore" @contact="goToContact" :isVisible="isSideNavVisible"></MySideNav>

        <img src="/imgSrc/logo.png" 
        class='scale-50 hover:scale-[0.60]'>

        <img src="/imgSrc/cart.svg" 
        class='scale-125 hover:scale-[1.6] pr-10 cursor-pointer active:scale-125'>
    </div>
    
</template>

<script>
import MySideNav from '../MySideNav.vue'
export default {
    data() {
        return {
            mobile: "mobile",
            isSideNavVisible: false,
        };
    },
    methods: {
        showSideNav() {
            this.isSideNavVisible = true
        },
        goToHome(){
            this.isSideNavVisible=false
            this.$emit('home')
        },
        goToExplore(){
            this.isSideNavVisible=false
            this.$emit('explore')
        },
        goToContact(){
            this.isSideNavVisible=false
            this.$emit('contact')
        }
    },
    components: { MySideNav }
}
</script>

<style>

img{
    @apply transition-all ease-in-out
}
.mobile{
    @apply text-cyan-700 text-6xl text-center
}
    
</style>
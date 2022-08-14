<template>

    <div 
    class="flex justify-between items-center 
    h-16 w-screen fixed z-50 bg-white md:h-20 
    lg:h-[5rem] lg:px-20">
        
        <img @click="showSideNav" src="/imgSrc/hamburger.svg" 
            class="hover:scale-[1.2] pl-10 cursor-pointer active:scale-100
            md:scale-150 md:hover:scale-[1.55] md:active:scale-150 lg:hidden
        ">
             
        <MySideNav @invisible="this.isSideNavVisible=false" @home="goToHome" @explore="goToExplore" @contact="goToContact" :isVisible="isSideNavVisible"></MySideNav>

        

        <img src="/imgSrc/logo.png" 
        class='scale-50 hover:scale-[0.60]
        md:scale-75 md:hover:scale-[0.80] 
        lg:scale-[0.7] lg:hover:scale-[0.75]'>

        <MyTopNav @home="goToHome" @explore="goToExplore" @contact="goToContact"></MyTopNav>

        <svg 
        class='scale-125 hover:scale-[1.6] mr-10 cursor-pointer active:scale-125 transition-all ease-in-out
        md:scale-[1.75] md:hover:scale-[1.95] md:active:scale-[1.75]'
        
        width="18" height="18" viewBox="0 0 18 18" fill="none" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
            <mask id="mask0_34_1088" style="mask-type:alpha" maskUnits="userSpaceOnUse" x="0" y="0" width="18" height="18">
            <rect width="18" height="18" fill="url(#pattern0)"/>
            </mask>
            <g mask="url(#mask0_34_1088)">
            <rect width="17.8" height="17.8" fill="black"/>
            </g>
            <defs>
            <pattern id="pattern0" patternContentUnits="objectBoundingBox" width="1" height="1">
            <use xlink:href="#image0_34_1088" transform="scale(0.0111111)"/>
            </pattern>
            <image id="image0_34_1088" width="90" height="90" xlink:href="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAFoAAABaCAYAAAA4qEECAAAABmJLR0QA/wD/AP+gvaeTAAADnElEQVR4nO2cv2sUQRTHP14wR8QEkTQSbRULO4laW9qK2NgIYhPTKJb+CwoqaK+N2MYYxYD4I/EXsRIllgGNGhWTCKfxzmISOMLO/rqZfbuz7wMD4WYy7+33Zt/Oj7cHiqIoiqIoEmwDrgM/gY6lLAGPgLPAgIyb1ecGdoGjykdgVMTTCtMAfpNN6A6wChwR8Ley5BW6AywAg8W7XB36uv7uAHuAgzn6GQJWgCcunKoDA8BV4AfZR/W8gL/B0gecxC72fjnXwuQ10UJfkHSqzDRy/t+E5fNjeR1RohklekT/BXYI+hUcDeAz0WKfEPSrtOQNHW1g0lKn4cMxx4ke0V/I/wUqEQwBLaLFPizoVynpZeT9Ap5Z6jR8bKLXW1yneQWxj+jQ0QZ2C/oVJPNEi31G0qkQuUK+rdWQyhJwGei3idRnq8hAGzjloJ8qM4CZaQ0CU1ENtjgw0gS+Adsd9FV1loDhqAoXC4sW8NBBPyFg1dPVCu6eo36qzlNbhSuhJzAPhbpjvbNdCf0JmHPUV5V5YKtwufljWyXWhQXgg61ShXbH/bhKl0K/AhYd9lc1YmdeLoVuk/CtBkwbmI5r4HqDvq7h4w1m0WbFtdBTwB/HfVYB62xjA9dCxx0GhEziytjH2V7dwscqMJvUSIXunWnMfk8sPoR+j0lQrwupNtR8pQXUaZMp8UEI/oSuS/iIXXZ340vox8Cyp77LROoFmi+hW5g3t0In9YGHz9St0MNH4rK7KHZhnJE+ofZVXmYRw+eIDv0wINVsYwPfWZ8hh49SHUgfQv4W91FWMGkWqfE9okM9DEi17O7Gt9ChHgZkDhtFZOaHGKczPQjBTUpYEkPAV2ISACvGAuZV7kwUMaJDOwzIFQqLeqknpPBRqmndZvYiPyVzUVrATsfaOOc58kL1Wu46V8UDR5EXqpeyBhxwroonbiIvWN5yyYMe3tgK3EFetKzlGsVMhZ3SAM5jjumlBUwq34HTfmQojmHgImbfYBH4h7ywa5jt3UlgDP1BLkVRFEVRlBw0gXFM6uvKepkFzpHxXK4idkUYAd5in9fOrbcJxa4ITeIvtvuiXY4wKbtijJN+xTYWgF0xXpD+gmcCsCvGMukv2GUKsIjdqvwQYLvqdiWFfuepbSntSgp9K0Pb2wHYFaOJmUKlmWa5TL6RsivKCPEX7XPBImFXlH7MfHUG85RfxqQmjOF3REnZVRRFURRFURRFKRf/AZ+eUXOMisFhAAAAAElFTkSuQmCC"/>
            </defs>
        </svg>

        <MyUnfilledBtn @click="login" id="login">Login</MyUnfilledBtn>

    </div>


    
</template>

<script>
import MySideNav from '../MySideNav.vue'
import MyTopNav from './MyTopNav.vue'
import MyUnfilledBtn from './MyUnfilledBtn.vue';
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
        },
        login(event){
            event.target.innerHTML='Logged'
        }
    },
    components: { MySideNav, MyTopNav, MyUnfilledBtn }
}
</script>

<style scoped>

img{
    @apply transition-all ease-in-out;
}
#login{
    @apply hidden lg:block transition-all ease-linear hover:bg-[#F14A16] hover:text-white rounded-2xl px-10 border-[2px] xl:text-sm
}

    
</style>
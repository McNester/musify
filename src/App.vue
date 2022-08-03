<template>
  <div class="overflow-hidden">

    
    <MyNavbar @explore="goToTrendsSection" @home="goToHeroSection" @contact="goToContactSection"></MyNavbar>

    <section ref="hero" id="heroSection">

      <div class="flex justify-end items-end w-[100vw] h-[100vh] absolute">
        <img class="hidden lg:block scale-[0.7] absolute -z-50 -mr-[8.3rem] mb-10" src="/imgSrc/heroPersonBack.png">
      </div>

      <h1 class="hero heroTitle">
        Let’s Dive in <br> <span id="orange" class="hero heroTitle">Music</span> World
      </h1>

      <h2 id="slogan" class="heroSlogan lg:hidden">
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc pharetra, phasellus
      </h2>

      <h2 id="slogan" class="heroSlogan hidden lg:block">
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc pharetra, phasellus imperdiet fringilla turpis lectus risus erat. Commodo purus, eu sed suspendisse fermentum
      </h2>

      

      <div class="flex w-full justify-start items-center">
        <MyFilledBtn>Shop now</MyFilledBtn>
        <MyUnfilledBtn id="heroUnfilledBtn">
          
          <svg width="23" height="22" viewBox="0 0 23 22" fill="none" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
          <mask id="mask0_34_1115" style="mask-type:alpha" maskUnits="userSpaceOnUse" x="0" y="0" width="23" height="22">
          <rect x="0.502441" y="0.197327" width="21.5247" height="21.5247" fill="url(#pattern0)"/>
          </mask>
          <g mask="url(#mask0_34_1115)">
          <rect x="0.502441" y="0.197327" width="21.2855" height="21.2855" fill="#F14A16"/>
          </g>
          <defs>
          <pattern id="pattern0" patternContentUnits="objectBoundingBox" width="1" height="1">
          <use xlink:href="#image0_34_1115" transform="scale(0.0111111)"/>
          </pattern>
          <image id="image0_34_1115" width="90" height="90" xlink:href="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAFoAAABaCAYAAAA4qEECAAAABmJLR0QA/wD/AP+gvaeTAAADnElEQVR4nO2cv2sUQRTHP14wR8QEkTQSbRULO4laW9qK2NgIYhPTKJb+CwoqaK+N2MYYxYD4I/EXsRIllgGNGhWTCKfxzmISOMLO/rqZfbuz7wMD4WYy7+33Zt/Oj7cHiqIoiqIoEmwDrgM/gY6lLAGPgLPAgIyb1ecGdoGjykdgVMTTCtMAfpNN6A6wChwR8Ley5BW6AywAg8W7XB36uv7uAHuAgzn6GQJWgCcunKoDA8BV4AfZR/W8gL/B0gecxC72fjnXwuQ10UJfkHSqzDRy/t+E5fNjeR1RohklekT/BXYI+hUcDeAz0WKfEPSrtOQNHW1g0lKn4cMxx4ke0V/I/wUqEQwBLaLFPizoVynpZeT9Ap5Z6jR8bKLXW1yneQWxj+jQ0QZ2C/oVJPNEi31G0qkQuUK+rdWQyhJwGei3idRnq8hAGzjloJ8qM4CZaQ0CU1ENtjgw0gS+Adsd9FV1loDhqAoXC4sW8NBBPyFg1dPVCu6eo36qzlNbhSuhJzAPhbpjvbNdCf0JmHPUV5V5YKtwufljWyXWhQXgg61ShXbH/bhKl0K/AhYd9lc1YmdeLoVuk/CtBkwbmI5r4HqDvq7h4w1m0WbFtdBTwB/HfVYB62xjA9dCxx0GhEziytjH2V7dwscqMJvUSIXunWnMfk8sPoR+j0lQrwupNtR8pQXUaZMp8UEI/oSuS/iIXXZ340vox8Cyp77LROoFmi+hW5g3t0In9YGHz9St0MNH4rK7KHZhnJE+ofZVXmYRw+eIDv0wINVsYwPfWZ8hh49SHUgfQv4W91FWMGkWqfE9okM9DEi17O7Gt9ChHgZkDhtFZOaHGKczPQjBTUpYEkPAV2ISACvGAuZV7kwUMaJDOwzIFQqLeqknpPBRqmndZvYiPyVzUVrATsfaOOc58kL1Wu46V8UDR5EXqpeyBhxwroonbiIvWN5yyYMe3tgK3EFetKzlGsVMhZ3SAM5jjumlBUwq34HTfmQojmHgImbfYBH4h7ywa5jt3UlgDP1BLkVRFEVRlBw0gXFM6uvKepkFzpHxXK4idkUYAd5in9fOrbcJxa4ITeIvtvuiXY4wKbtijJN+xTYWgF0xXpD+gmcCsCvGMukv2GUKsIjdqvwQYLvqdiWFfuepbSntSgp9K0Pb2wHYFaOJmUKlmWa5TL6RsivKCPEX7XPBImFXlH7MfHUG85RfxqQmjOF3REnZVRRFURRFURRFKRf/AZ+eUXOMisFhAAAAAElFTkSuQmCC"/>
          </defs>
          </svg>


          <h1>Add to cart</h1>

        </MyUnfilledBtn>
      </div>

      <div 
      class="flex flex-col justify-center items-center gap-10 pb-10 
      lg:flex-row-reverse lg:justify-around lg:w-screen">
      
        <div class="grid grid-cols-3 gap-[15rem] 
        py-7 overflow-y-hidden overflow-x-scroll w-screen -ml-5
        md:py-20 lg:gap-0 lg:w-[59vw] lg:overflow-hidden lg:py-0 lg:mb-10">
            <MyHeadphonesCard></MyHeadphonesCard>
            <MyHeadphonesCard></MyHeadphonesCard>
            <MyHeadphonesCard></MyHeadphonesCard>
        </div>

        <button @click="goToTrendsSection" 
        class="self-center -ml-5 animate-bounce lg:animate-none flex justify-center items-center transition-all ease-in-out
        sm:mb-[10%] sm:mt-[10%] 
        lg:mt-[13rem] lg:hover:scale-105 lg:active:scale-100 lg:w-1/3 ">
          <svg class="scale-90 sm:scale-[1.2]" width="76" height="76" viewBox="0 0 76 76" fill="none" xmlns="http://www.w3.org/2000/svg">
            <g filter="url(#filter0_d_34_1142)">
            <circle cx="38" cy="36" r="29.5" stroke="#1E1E1E"/>
            <path d="M38 52L43.7735 42L32.2265 42L38 52ZM37 20L37 43L39 43L39 20L37 20Z" fill="#1E1E1E"/>
            </g>
            <defs>
            <filter id="filter0_d_34_1142" x="0" y="0" width="76" height="76" filterUnits="userSpaceOnUse" color-interpolation-filters="sRGB">
            <feFlood flood-opacity="0" result="BackgroundImageFix"/>
            <feColorMatrix in="SourceAlpha" type="matrix" values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0" result="hardAlpha"/>
            <feOffset dy="2"/>
            <feGaussianBlur stdDeviation="4"/>
            <feComposite in2="hardAlpha" operator="out"/>
            <feColorMatrix type="matrix" values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.6 0"/>
            <feBlend mode="normal" in2="BackgroundImageFix" result="effect1_dropShadow_34_1142"/>
            <feBlend mode="normal" in="SourceGraphic" in2="effect1_dropShadow_34_1142" result="shape"/>
            </filter>
            </defs>
          </svg>
        </button>

      </div>

    </section>

    <section ref="trends" id="trendsSection" 
    class="flex flex-col mx-auto justify-center items-center
           w-screen">
      <h1 id="trendsTitle">Popular trends</h1>

      <div class="grid grid-cols-5 gap-[15rem] py-7 overflow-y-hidden overflow-x-scroll w-screen pl-5">
         <MyTrendsHeadphonesCard></MyTrendsHeadphonesCard>
         <MyTrendsHeadphonesCard></MyTrendsHeadphonesCard>
         <MyTrendsHeadphonesCard></MyTrendsHeadphonesCard>
         <MyTrendsHeadphonesCard></MyTrendsHeadphonesCard>
         <MyTrendsHeadphonesCard></MyTrendsHeadphonesCard>
         
      </div>
    </section>
    
    <section id="buySection">
      <MyWhyCard></MyWhyCard>
    </section>

    <section v-if="isOfferActive" id="offerSection">
      <h1 id="offerTitle">Exclusive offer</h1>
      <div class="relative">
        <div id="discount">
          <h1>20% <br>off</h1>
        </div>
        <img src="/imgSrc/offerHeadphones.png" class="">
      </div>

      <div id="timerOffer">
          <h1>Offer ends in</h1>
          <MyTimer @offerEnd="removeOfferSection"></MyTimer>
          <div class="flex justify-between items-center w-full">
            <MyUnfilledBtn id="offerDetails">View deatails</MyUnfilledBtn>
            <MyFilledBtn id="offerShop">Shop now</MyFilledBtn>
          </div>
      </div>
    </section>

    <section id="otherAccessories">
      <h1 class="mt-10 w-[90vw]">Try our other Accessories</h1>
      <div id="accessoriesContainer">
        <img src="/imgSrc/watch.png">
        <img src="/imgSrc/siri.png">
        <img src="/imgSrc/soundbar.png">
        <img src="/imgSrc/home.png">
      </div>
    </section>

    <section id="arrivalsSection">
      <h1 id="trendsTitle">New Arrivals</h1>

      <div class="grid grid-cols-3 gap-[20rem] py-7 overflow-y-hidden overflow-x-scroll w-screen pl-5 mr-5">
        <MyArrivalsCard>
          <img src="/imgSrc/arrivalOne.png" class="scale-[1]">
        </MyArrivalsCard>

        <MyArrivalsCard>
          <img src="/imgSrc/arrivalTwo.png" class=" rounded-t-[2.9rem] h-[51%]">
        </MyArrivalsCard>
        <MyArrivalsCard>

          <img src="/imgSrc/arrivalThree.png" class=" rounded-t-[2.9rem] h-[51%]">
        </MyArrivalsCard>


      </div>
    </section>

    <section id="qrSection">
      <MyQRCard></MyQRCard>
    </section>

    <footer ref="contact" class="pt-12">
      <MyFooter></MyFooter>
    </footer>

  </div>
</template>

<script>
import MyNavbar from './components/UI/MyNavbar.vue';
import MyFilledBtn from './components/UI/MyFilledBtn.vue';
import MyUnfilledBtn from './components/UI/MyUnfilledBtn.vue';
import MyHeadphonesCard from './components/UI/MyHeadphonesCard.vue';
import smoothscroll from 'smoothscroll-polyfill';
import MyTrendsHeadphonesCard from './components/UI/MyTrendsHeadphonesCard.vue';
import MyWhyCard from './components/MyWhyCard.vue';
import MyTimer from './components/MyTimer.vue';
import MyArrivalsCard from './components/UI/MyArrivalsCard.vue';
import MyQRCard from './components/MyQRCard.vue';
import MyFooter from './components/UI/MyFooter.vue';

export default{
  components: { MyNavbar, MyFilledBtn, MyUnfilledBtn, MyHeadphonesCard, MyTrendsHeadphonesCard, MyWhyCard, MyTimer, MyArrivalsCard, MyQRCard, MyFooter },
  methods:{
    goToTrendsSection(){
      var element = this.$refs['trends']
      var elTop = element.offsetTop

      smoothscroll.polyfill();
      window.scrollTo({top:elTop,behavior: 'smooth'})
    },
    goToHeroSection(){
      var element = this.$refs['hero']
      var elTop = element.offsetTop

      smoothscroll.polyfill();
      window.scrollTo({top:elTop,behavior: 'smooth'})
    },
    goToContactSection(){
      var element = this.$refs['contact']
      var elTop = element.offsetTop

      smoothscroll.polyfill();
      window.scrollTo({top:elTop,behavior: 'smooth'})
    },
    removeOfferSection(){
      this.isOfferActive = false
    }
  },
  data() {
    return {
      isOfferActive: true
    }
  },
}

</script>


<style>
html{
  background: transparent;
}
@font-face {
  font-family: proxima;
  src: url('/Proxima Nova/proximanova_regular.ttf');
}
@font-face {
  font-family: proximaBold;
  src: url('/Proxima Nova/proximanova_bold.otf');
}
@font-face {
  font-family: proximaLight;
  src: url('/Proxima Nova/proximanova_light.otf');
}

.hero{
  font-family: proximaBold;
}
.heroTitle{
  @apply text-6xl text-left w-screen
}
#orange{
  color: #F14A16;
}
#slogan{
  font-family: proximaLight;
}
.heroSlogan{
  @apply text-xl text-left w-[90%] text-[#282828]/50 lg:w-[35rem]
}
#heroSection{
  @apply flex flex-col ml-5 gap-5 items-start justify-center w-screen mt-20 lg:mt-48 lg:relative
}
#heroUnfilledBtn{
  font-family: proximaBold;
  @apply ml-10
}
#trendsTitle{
  font-family: proximaBold;
  @apply text-5xl md:text-6xl
}

#buySection{
  @apply flex justify-center items-center mt-10
}

#offerSection{
  @apply scale-[0.9] flex justify-center items-center flex-col gap-20 relative
}
#offerTitle{
  font-family: proximaBold;
  @apply text-5xl mt-20 md:text-6xl
}
#discount{
  font-family: proximaBold;
  @apply h-[7rem] w-[7rem] bg-[#370665] 
  absolute rounded-[100rem] flex justify-center items-center text-white
  text-4xl text-center shadow-2xl 
  
}
#timerOffer{
  font-family: proxima;
  @apply flex flex-col text-4xl justify-center items-center gap-5
}
#offerDetails{
  font-family: proximaLight;
  @apply text-xl shadow-[#F14A16] shadow-[0px_0px_20px_-4px]
}
#offerShop{
  @apply shadow-[#F14A16] shadow-[0px_10px_20px_-5px] text-xl
}

#otherAccessories{
  font-family: proximaBold;
  @apply flex flex-col justify-center items-center text-4xl text-center gap-10 md:text-5xl
}
#otherAccessories img{
  @apply scale-90 hover:scale-95 active:scale-90 cursor-pointer transition-all ease-in-out
}
#accessoriesContainer{
   @apply grid justify-center items-center md:grid-cols-2
}
#arrivalsSection{
  @apply flex justify-center items-center flex-col mx-auto w-screen mt-10
}

#qrSection{
  @apply mt-20 flex justify-center items-center mb-20
}
</style>

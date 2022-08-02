<template >
    <div class=" flex flex-col bg-[#370665] rounded-[3.1rem] justify-start items-center w-[19rem] h-[36.5rem] border-[#35589A] border-4">
        <slot></slot>
        <div class="flex flex-col justify-start bg-[#370665] rounded-b-[2rem]">
            <h1 class="text-md ml-4 mt-5">
                Wireless Headphones with Dolby Surround Sound
            </h1>
            
            <li class="mt-5">Truely Wireless</li>
            <li>Dolby Surround Sound</li>
            <li>13hrs of playback time</li>
            <li>Made in Germany</li>

            <h1 id="price" class="mt-4 ml-4 text-xl">$145</h1>

            <div class="flex w-[100%] self-center justify-between items-center relative">
                <MyUnfilledBtn id="btnFirst">
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


                    <h1 class="unfilledBtn">Add to cart</h1>
                </MyUnfilledBtn>

                <MyFilledBtn id="btnSecond">
                    <h1 class="unfilledBtn">Buy now</h1>
                </MyFilledBtn>

                
            </div>
            
        </div>
    </div>
</template>

<script>
import MyUnfilledBtn from './MyUnfilledBtn.vue';
import MyFilledBtn from './MyFilledBtn.vue';
export default {
    components: { MyUnfilledBtn, MyFilledBtn }
}
</script>

<style scoped >
*{
    font-family: proxima;
    color: white;
}
li{
    @apply text-[0.8rem] mt-2 ml-5
}
#price{
    color: #FC9918;
}
.unfilledBtn{
    font-family: proximaBold;
}
#btnFirst{
    @apply scale-[0.70] absolute left-0 top-0 hover:scale-[0.75] active:scale-[0.70]
}
#btnSecond{
    @apply scale-[0.70] absolute right-0 top-0 ml-10 hover:scale-[0.75] active:scale-[0.70] shadow-[#F14A16] shadow-[0px_0px_50px_-5px]
}
</style>
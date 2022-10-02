<template>
<div>


    <div id="bg-brackets" v-for = "idx in 50" :key = "idx" style = "position: absolute;width: 100vw;overflow: hidden;">
        <SlidingBrackets text = "</>" :top = "Math.floor(Math.random()*100).toString()" :time = "Math.floor(Math.random()*10+3).toString()" :offset = "(Math.floor(Math.random()*20) - 20).toString()"></SlidingBrackets>
    </div>
    <!-- <SlidingBrackets text="</html>" top = "90" time="7"></SlidingBrackets>
    <SlidingBrackets text="#id" top = "10" time="5"></SlidingBrackets>
    <SlidingBrackets text="{coding}" top = "45" time="10"></SlidingBrackets> -->

    <div class = "top-section  px-[10%]  flex flex-col  min-h-[50vh] justify-center mb-5">
        <div class="left-section ">


            <div class = " hidden sm:block -z-1 text-[6rem] bg-white  border-4 border-white text-white opacity-30 left-[0vw] absolute w-[100vw]">
                .
            </div>
            <div class = "text-[3rem] sm:text-[6rem] text-white z-10 text-center">
                Web Developer
            </div>

            <p class=" text-xl top-text sm:text-4xl pt-6 text-center">
                Learning something great about the web everyday...
            </p>

            <div class="my-toolkit text-center  mt-[50px]">
                <h1 class="underline text-2xl sm:text-3xl mt-5">My Comfort Zone</h1>
                <h1 class="text-sm sm:text-2xl mb-5">a.k.a cool things ive used before</h1>

                <div class="logos grid">
                    <div class="logo-container">
                        <img class=" w-[30px] md:w-[50px] h-[30px] md:h-[50px]"  src="~/assets/images/js.png" >

                    </div>
                    <div class="logo-container">
                        <img class=" w-[30px] md:w-[50px] h-[30px] md:h-[50px]"  src="~/assets/images/react.webp" >

                    </div>
                    <div class="logo-container">

                        <img class=" w-[30px] md:w-[50px] h-[30px] md:h-[50px]"  src="~/assets/images/vue.png" >
                    </div>
                    <div class="logo-container">

                        <img class=" w-[30px] md:w-[50px] h-[30px] md:h-[50px]"  src="~/assets/images/nuxt.webp" style="transform:scale(1.6);">
                    </div>
                    <div class="logo-container">
                        <img class=" w-[30px] md:w-[50px] h-[30px] md:h-[50px]"  src="~/assets/images/firebase.png" >

                    </div>
                    <div class="logo-container">

                        <img class=" w-[30px] md:w-[50px] h-[30px] md:h-[50px]"  src="~/assets/images/sql.png" >
                    </div>
                    <div class="logo-container">
                        <img class=" w-[30px] md:w-[50px] h-[30px] md:h-[50px]"  src="~/assets/images/python.png" >

                    </div>
                    <div class="logo-container">
                        <img class=" w-[30px] md:w-[50px] h-[30px] md:h-[50px]"  src="~/assets/images/cpp.png" >

                    </div>
                    <div class="logo-container">
                        <img class=" w-[30px] md:w-[50px] h-[30px] md:h-[50px]"  src="~/assets/images/flask.png" >

                    </div>
                </div>
            </div>
        </div>

        
        
        
        <NuxtLink to="/about" class="about-me underline justify-center mx-auto text-xl sm:text-3xl mt-12">
            Read More about me!
        </NuxtLink>
    </div>


</div>
</template>

<style>
@media(min-width: 640px){

    .logos {
        grid-auto-flow: column;
    }
}
@media(max-width : 640px){
    .logos{
        grid-template-columns: repeat(3, 1fr) !important;
        justify-items: center;
        align-items: center;
    }
}

.logo-container > img{
    margin: 10px;
}

.logo-container{
    background: rgba(250, 250, 250, 0.7);
    margin: 10px;
    border-radius: 5px;
    width: fit-content;
    
}
.logo-container:hover {
    animation: scaleup 0.5s ease forwards;
}
.logo-container:not(:hover) {
    animation: scaledown 0.5s ease forwards;
    animation-delay: 1s;
}

@keyframes scaleup {
    100% {
        transform: scale(1.2);

    }
}
@keyframes scaledown {
    0% {
        transform: scale(1.2);

    }
    100% {
        transform: scale(1);
    }
}
</style>
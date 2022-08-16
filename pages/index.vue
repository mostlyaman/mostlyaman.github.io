<template>
<div>


    <div id="bg-brackets" v-for = "idx in 50" :key = "idx" style = "width: 100vw;overflow: hidden;">
        <SlidingBrackets text = "</>" :top = "Math.floor(Math.random()*100).toString()" :time = "Math.floor(Math.random()*10+3).toString()" :offset = "(Math.floor(Math.random()*20) - 20).toString()"></SlidingBrackets>
    </div>
    <!-- <SlidingBrackets text="</html>" top = "90" time="7"></SlidingBrackets>
    <SlidingBrackets text="#id" top = "10" time="5"></SlidingBrackets>
    <SlidingBrackets text="{coding}" top = "45" time="10"></SlidingBrackets> -->

    <div class = "top-section  px-[10%]  flex flex-row">
        <div class="left-section basis-1/2">


            <div class = " -z-1 text-[6rem] bg-white  border-4 border-white text-white opacity-30 left-[0vw] absolute w-[100vw]" style="">
                .
            </div>
            <div class = "text-[6rem] text-white z-10">
                Web Developer
            </div>

            <p class="top-text  basis-1/2 text-4xl pt-6 text-center">
                Learning something great about the web everyday...
            </p>
        </div>

    </div>


</div>
</template>

<style>

</style>
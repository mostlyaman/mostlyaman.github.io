<template>
    <div>
    
    
        <div id="bg-brackets" v-for = "idx in 50" :key = "idx" style = "position: absolute;width: 100vw;overflow: hidden;">
            <SlidingBrackets text = "</>" :top = "Math.floor(Math.random()*100).toString()" :time = "Math.floor(Math.random()*10+3).toString()" :offset = "(Math.floor(Math.random()*20) - 20).toString()"></SlidingBrackets>
        </div>
        <!-- <SlidingBrackets text="</html>" top = "90" time="7"></SlidingBrackets>
        <SlidingBrackets text="#id" top = "10" time="5"></SlidingBrackets>
        <SlidingBrackets text="{coding}" top = "45" time="10"></SlidingBrackets> -->
    
        <div class = "top-section  px-[10%]  flex flex-col  min-h-[50vh] justify-center mb-5">
            <div class = "text-[3rem] sm:text-[6rem] text-white z-10 text-center underline">
                Hi, im Aman
            </div>
            <div class="text text-2xl">
                <p class=" m-4 text-center">
                    Web Developer and Student from India. I like to make fast and beautiful web apps for people 
                </p>
                <p class=" m-4 text-center">Lorem ipsum dolor, sit amet consectetur adipisicing elit. Iste optio veritatis illum repudiandae odit dignissimos ducimus earum in praesentium laboriosam possimus magnam fuga vitae nam reprehenderit, et eaque obcaecati maiores? Consectetur, ad neque, ab exercitationem hic expedita fuga eos facilis dolores sed natus corrupti repellat deserunt itaque laborum molestiae id!</p>
            </div>
        </div>
    
    
    </div>
    </template>
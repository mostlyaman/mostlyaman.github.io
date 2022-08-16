<template>
    <div id = "div" :style = "{'opacity': '0.7','position': 'fixed','top': top + 'vh', 'animation': `example ${time}s linear infinite`, 'animation-delay': `${offset}s`, 'z-index': '-1'}" class="text-2xl text-gray-300">
        {{ text }}
    </div>
</template>

<script>
export default {
    name: "SlidingBrackets",
    props: {
        text: String,
        top: String,
        time: String,
        offset: String
    }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Rubik+Moonrocks&display=swap');
#div {
    font-family: 'Rubik Moonrocks', cursive;
}



</style>
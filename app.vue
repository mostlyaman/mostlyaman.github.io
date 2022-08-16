<template>
  <div>
    <NuxtLayout>
      <NuxtPage/>
    </NuxtLayout>
  </div>
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Lobster+Two&display=swap');


* {
  font-family: "Lobster Two", Arial, Helvetica, sans-serif;
  box-sizing: border-box;
}

@keyframes example {
  from {left: -10vw;}
  to {left: 100vw;}
}

body {
  color: white;
  width: 100vw;
  height: 100vh;
  overflow: hidden;


	background: linear-gradient(-45deg, #ee7752, #e73c7e, #23a6d5, #23d5ab);
	background-size: 400% 400%;
	animation: gradient 15s ease infinite;
	height: 100vh;
}

@keyframes gradient {
	0% {
		background-position: 0% 50%;
	}
	50% {
		background-position: 100% 50%;
	}
	100% {
		background-position: 0% 50%;
	}
}



</style>
<template>
    <div class = "container w-screen px-12 py-4 flex justify-between items-center mx-auto">

        <!-- Logo -->
        <div id = "logo" class = "logo text-xl sm:text-4xl">
            mostlyaman.dev
        </div>

        <div>
            <ul class = "flex text-lg sm:text-2xl">
                <NuxtLink to="/about" class="hover:underline">About Me</NuxtLink>
                <NuxtLink to="/contact" class="hover:underline">Contact</NuxtLink>

            </ul>
        </div>

    </div>
</template>

<script setup>

</script>

<style scoped>

li:hover{
    cursor: pointer;
    text-decoration: underline;
}

li, a {
    margin: 0px 20px;
}





</style>
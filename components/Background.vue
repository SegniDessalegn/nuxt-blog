<template>
    <div class="absolute red-shadow"></div>
    <div class="absolute blue-shadow"></div>
</template>

<style scoped>
.red-shadow {
    position: absolute;
    top: 50%;
    left: 25%;
    border-radius: 50%;
    box-shadow: 0 0 350px 250px rgba(97, 3, 22, 0.15);
}
.blue-shadow {
    position: absolute;
    bottom: 10%;
    right: 25%;
    border-radius: 50%;
    box-shadow: 0 0 350px 250px rgba(3, 3, 97, 0.25);
}
</style>

<template>
    <nav class="navbar">
        <div class="">
            <nuxt-link class="text-2xl font-bold text-blue-500" to="/">Segni Blogs</nuxt-link>
        </div>
        <div class="flex justify-end items-center gap-5">
            <ThemeSwitcher />
        </div>
    </nav>
</template>

<style lang="postcss">
.navbar {
    background-color: #fff;
    /* Set your navbar background color */
    color: #333;
    /* Set your navbar text color */
    padding: 10px 20px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    position: sticky;
    top: 0px;
    left: 0px;
    z-index: 10;
}

body {
    @apply min-h-screen bg-white dark:bg-gray-800 dark:text-gray-200;
}

div, p, nav, main {
    @apply bg-white dark:bg-gray-800 dark:text-gray-200;
}
</style>

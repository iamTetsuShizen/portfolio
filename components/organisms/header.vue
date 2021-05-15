<template>
    <header class="header">
        <div class="logo">
            <picture>
                <img >
            </picture>
        </div>
        <nav class="menu">
            <ul class="menu__list">
                <li class="menu__item"  v-for="menuItem in menu" :key="menuItem.key">
                    <NuxtLink :to="{ path: menuItem.url }"> {{ menuItem.name }}</NuxtLink>
                </li>
            </ul>
        </nav>
    </header>
</template>

<script>
import menuUrls from '../../config/menu.json';


export default {
    data() {
        return {
            menu : menuUrls
        }
    }
}
</script>

<style scoped>
    .test {
        background-color: red;
    }
</style>
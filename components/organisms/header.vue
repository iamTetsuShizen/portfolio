<template>
    <header class="header">
        <div class="header__logo">
            <picture>
                <img >
            </picture>
        </div>
        <nav class="header__menu">
            <ul class="header__menu-list">
                <li class="header__menu-list-item"  v-for="menuItem in menu" :key="menuItem.key">
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
<script setup>
import { RouterLink } from 'vue-router';

</script>

<template>
    <nav>
        <div class="nav-bar">
            <RouterLink to="/">
                <img src="../assets/folha.png" alt="Folha de árvore" class="nav-logo">
            </RouterLink>
            <ul>
                <li><RouterLink to="/">Home</RouterLink></li>
                <li><RouterLink to="/sobre">Sobre</RouterLink></li>
            </ul>
        </div>
    </nav>
</template>

<style scoped>
.nav-bar {
    width: 100%;
    height: 6vh;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
    padding: 20px;
    background: var(--color-navbar);
}

.nav-logo {
    width: 40px;
    height: 40px;
}

ul {
    width: 12vw;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    list-style: none;
}

ul li a {
    color: var( --color-text);
    font-weight: bold;
    text-decoration: none;
}

ul li a:hover {
    cursor: pointer;
    color: var( --color-text-focus);
    text-decoration: none;
}
</style>
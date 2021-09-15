<template>
    <div class="navigation">
        <ul class="navigation-list">
            <li class="navigation-list__item">
                <a href="#home" @click="$emit('navigationToggled', $event)" class="navigation-list__link">
                    Home
                </a>
            </li>
            <li class="navigation-list__item">
                <a href="#services" @click="$emit('navigationToggled', $event)" class="navigation-list__link">
                    My Services
                </a>
            </li>
            <li class="navigation-list__item">
                <a href="#about" @click="$emit('navigationToggled', $event)" class="navigation-list__link">
                    About me
                </a>
            </li>
            <li class="navigation-list__item">
                <a href="#work" @click="$emit('navigationToggled', $event)" class="navigation-list__link">
                    My Work
                </a>
            </li>
        </ul>
    </div>
</template>

<script>
export default {
    name: "Navigation"
}
</script>

<style scoped>
.navigation {
    height: 100vh;
}

.navigation-list {
    display: flex;
    flex-direction: column;
    list-style: none;
    justify-content: space-around;
    height: 100%;
}

.navigation-list__item {
    background: #000000;
    display: flex;
    align-items: center;
    justify-content: center;
    height: 100%;
    width: 100%;
    color: #ffffff;
}

.navigation-list__link {
    color: inherit;
    text-decoration: none;
}
</style>
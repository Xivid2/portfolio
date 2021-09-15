<template>
    <div class="header">
        <div class="logo">
            <img src="../assets/images/logo.png" alt="logo" />
        </div>
        <button
            @click="$emit('navigationToggled', $event)"
            class="nav-toggle"
            aria-label="toggle navigation"
            >
            <span class="hamburger"></span>
        </button>
    </div>
</template>

<script>

export default {
    name: "Header"
}
</script>

<style scoped>
.nav-toggle {
    height: 20px;
    width: 20px;
}
</style>



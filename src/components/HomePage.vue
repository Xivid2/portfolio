<template>
    <div v-if="navigationToggled" id="home">
        <Navigation
            
        />
    </div>
    <div v-else>
        <Header
            @navigationToggled = toggleNavigation()
        />
    </div>
</template>

<script>
import Header from "./Header.vue";
import Navigation from "./Navigation.vue";

export default {
    name: "HomePage",
    components: {
        Header,
        Navigation
    },
    data() {
        return {
            navigationToggled: false
        }
    },
    methods: {
        toggleNavigation() {
            this.navigationToggled = !this.navigationToggled;
        }
    }
};
</script>

<style scoped lang="scss">
    
</style>

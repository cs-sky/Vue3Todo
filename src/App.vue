<template>
    <v-app>
        <div>
            <v-toolbar>
                <v-toolbar-title>Vue 3 Examples</v-toolbar-title>

                <div class="flex-grow-1"></div>

                <v-toolbar-items>
                    <v-btn :to="{ name: 'home'}" text>Home</v-btn>
                    <v-btn :to="{ name: 'sf'}" text>Functional Components</v-btn>
                </v-toolbar-items>
            </v-toolbar>
        </div>

        <router-view>
            <home />
        </router-view>
    </v-app>
</template>

<script>
import Home from "./components/Home.vue";

export default {
    name: "App",
    components: {
        Home
    }
};
</script>

<style>
body {
    font-family: "Roboto, sans-serif";
}

.v-btn:not(.v-btn--round).v-size--large {
    font-size: 40px;
}
</style>

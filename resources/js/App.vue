<template>
    <div class="app">
        <Navbar />
        <hr />
        <div class="content">
            <router-view />
        </div>
    </div>
</template>

<script>
import Navbar from "./components/Navbar";
export default {
    name: "App",

    components: {
        Navbar,
    },
};
</script>

<style>
:root {
    --primary: #ddd;
    --dark: #333;
    --light: #fff;
    --shadow: 0 1px 5px rgba(104, 104, 104, 0.8);
}
</style>

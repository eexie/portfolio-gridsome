<template>
    <footer class="footer">
        <div class="container">
            <g-link class="nav__link" to="/about">About</g-link>
            <g-link class="nav__link" to="https://www.figma.com/proto/TOrH5UHfJxbovU2WZP8yZf/Resume?node-id=1%3A2&scaling=min-zoom&page-id=127%3A92&starting-point-node-id=1%3A2">Resume</g-link>
            <!--<g-link class="nav__link" to="/journal">Journal</g-link>
            <g-link class="nav__link" to="/contact">Say Hi!</g-link>-->
            <span v-html="settings.footer" />
        </div>
    </footer>
</template>

<script>
export default {
    data() {
        return {
            settings: require("../../data/theme.json")
        }
    }
}
</script>

<style scoped>
.footer {
    font-size: 0.8rem;
    padding: 6rem 0;
}
</style>

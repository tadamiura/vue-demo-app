<template>
    <div id="nav">
        <span 
        v-for="(viewPath,viewName) in views" :key="viewName"
        class="nav-element"
        >
            <router-link :to='viewPath'>{{viewName}}</router-link>  
        </span>
    </div>
</template>
<script>
export default {
    name: 'TheNavbar',
    data() {
        return {
            views: {
            Home: '/',
            About: '/about',
            Popper: '/popper'
            }
        }
    },
}
</script>
<style scoped>
.nav-element {
    margin: 0 7px;
}
</style>
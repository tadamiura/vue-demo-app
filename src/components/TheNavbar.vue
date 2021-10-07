<template>
    <div id="nav">
        <div v-for="(viewPath,viewName) in views" :key="viewName">
            <router-link :to='viewPath'>{{viewName}}</router-link>  |
        </div>
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
<script>
import NavLink from './NavLink.vue';

export default {
    name: 'AppHeader',
    components: {
        NavLink,
    },
    data() {
        return {
            navbarLinks: [
                { name: 'Gino', link: '#' },
                { name: 'Ciao', link: '#' },
                { name: 'Home', link: '#' },
                { name: 'Contatti', link: '#' },
                { name: 'Ginetta', link: '#' },
            ],
        };
    },
}
</script>



<script setup>
    import NavLink from './NavLink.vue';
</script>

<template>
    <header>
        <nav>
            <ul>
                <li v-for="link in navbarLinks" :key="link.name">
                    <NavLink :name="link.name" :link="link.link" />
                </li>
            </ul>
        </nav>
    </header>
</template>


<style scoped>
ul{
    display: flex;
    justify-content: space-around;
    align-items: center;
    flex-direction: row;
    flex-wrap: wrap;
    list-style: none;
    padding: 10px;
    font-size: x-large;
}

</style>

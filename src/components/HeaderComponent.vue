<template>
    <header class="container text-center ">
        <img src="/images/la-molisana-logo.png" alt="La Molisana logo" />

        <ul>
            <li class="list-unstyled " v-for="item in menu" :key="item.name">
                <a :href="item.url">{{ item.name }}</a>
            </li>
        </ul>
    </header>
</template>

<script>
    export default {
        name: 'HeaderComponent',
        data() {
            return {
                menu: [
                    { name: 'Home', url: '#' },
                    { name: 'Prodotti', url: '#' }, 
                    { name: 'Chi siamo', url: '#' }, 
                    { name: 'Contatti', url: '#' }, 
                ],
            };
        },
    };
</script>

<style lang="scss" scoped>
ul{
    display: flex;
    justify-content: center;

    li{
        margin: 0 10px;
        list-style: none;
    }
}

    /* Add your styles here */
</style>
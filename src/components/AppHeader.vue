<script>
    export default {
        data() {
            return {
                navbar:[
                    {
                        label:'Characters',
                        url: '#',
                        active : false
                    },
                    {
                        label:'Comics',
                        url: '#',
                        active : true
                    },
                    {
                        label:'Movies',
                        url: '#',
                        active : false
                    },
                    {
                        label:'TV',
                        url: '#',
                        active : false
                    },
                    {
                        label:'Games',
                        url: '#',
                        active : false
                    },
                    {
                        label:'Colletibles',
                        url: '#',
                        active : false
                    },
                    {
                        label:'Videos',
                        url: '#',
                        active : false
                    },
                    {
                        label:'Fans',
                        url: '#',
                        active : false
                    },
                    {
                        label:'News',
                        url: '#',
                        active : false
                    },
                    {
                        label:'Shop',
                        url: '#',
                        active : false
                    }
                    ]
            }
        },
    }
</script>

<template lang="">
    <header>
        <a href="/" class="brand">
                <img src="../assets/vue-dc-comics-1/img/dc-logo.png" alt="logo">
        </a>
        <nav>
            <ul>
                <li v-for="(item, index) in navbar" :key="index">
                    <a :href="item.url" :class="item.active ? 'active' : ''">
                    {{item.label}}</a>
                </li>
            </ul>
        </nav>
    </header>
</template>

<style scoped lang="scss">
    @use '../styles/partials/variables' as *;
    @use '../styles/partials/mixins' as *;

    header{
        display: flex;
        a img {
            padding: 1rem;
            height: 80%;
        }
    }
    ul{
        list-style: none;
        margin: 2rem 1rem;
        @include center;
        li a {
            display:inline-block;
            padding: 1rem;
            text-decoration: none;
            font-size:13px;

            &.active, &:hover{
                color: $primary;
                border-bottom: 3px solid $primary;
                
            }
        }
    }

</style>

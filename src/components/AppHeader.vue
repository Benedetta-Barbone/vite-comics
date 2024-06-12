<script> 
    export default{
        name: 'AppHeader',
        data (){
            return {
                option : [
                    {
                        id: 1,
                        title: 'CHARACTERS',
                        visible: true
                    },
                    {
                        id: 2,
                        title: 'MOVIES',
                        visible: true
                    },
                    {
                        id: 3,
                        title: 'TV',
                        visible: true
                    },
                    {
                        id: 4,
                        title: 'GAMES',
                        visible: true
                    },
                    {
                        id: 5,
                        title: 'COLLECTIBLES',
                        visible: true,
                    },
                    {
                        id: 6,
                        title: 'VIDEOS',
                        visible: true
                    },
                    {
                        id: 7,
                        title: 'FANS',
                        visible: true
                    },
                    {
                        id: 8,
                        title: 'NEWS',
                        visible: true
                    },
                    {
                        id: 9,
                        title: 'SHOP',
                        visible: true
                    }
                ]
            }
        }
    }
</script>

<template> 
<header>
    <div>
        <img src="/img/dc-logo.png" alt="">
        <ul>
            <li  v-for="index in option" :key="index.id">
                {{ index.title }}
            </li>
        </ul>
    </div>
</header>
</template>

<style lang="scss" scoped>
    @use '../styles/partials/variables' as *;
    @use '../styles/partials/mixins' as *;
    @use '../styles/general.scss' as *;

header div{
    background-color: white;
    display: flex;
    justify-content: space-between;
    margin: 0 auto;
    width: 70%;
    font-size: 12px;
    padding: 1rem 0rem;


    img{
        width: 70px;
    }

    ul{
        display: flex;
        

        li{
            padding: 1rem;
        }
    }
}


</style>
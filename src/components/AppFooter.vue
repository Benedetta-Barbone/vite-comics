<script> 
export default{
        name: 'AppFooter',
        data (){
            return {
                options : [
                    {
                        id: 1,
                        title: 'DIGITAL COMICS',
                        image: 'img/buy-comics-digital-comics.png',
                        visible: true
                    },
                    {
                        id: 2,
                        title: 'MOVIES',
                        image: 'img/buy-comics-merchandise.png',
                        visible: true
                    },
                    {
                        id: 3,
                        title: 'TV',
                        image: 'img/buy-comics-shop-locator.png',
                        visible: true
                    },
                    {
                        id: 4,
                        title: 'GAMES',
                        image: 'img/buy-comics-subscriptions.png',
                        visible: true
                    },
                    {
                        id: 5,
                        title: 'COLLECTIBLES',
                        image: 'img/buy-dc-power-visa.svg',
                        visible: true,
                    },
                ],
                dcComics : [
                    {
                        id: 1,
                        title: 'Characters',
                        visible: true
                    },
                    {
                        id: 2,
                        title: 'Comics',
                        visible: true
                    },
                    {
                        id: 3,
                        title: 'Movies',
                        visible: true
                    },
                    {
                        id: 4,
                        title: 'TV',
                        visible: true
                    },
                    {
                        id: 5,
                        title: 'Games',
                        visible: true,
                    },
                    {
                        id: 6,
                        title: 'Videos',
                        visible: true,
                    },
                    {
                        id: 7,
                        title: 'News',
                        visible: true,
                    },
                ],
                shop : [
                    {
                        id: 1,
                        title: 'Shop DC',
                        visible: true
                    },
                    {
                        id: 2,
                        title: 'Shop DC collectibles',
                        visible: true
                    },
                ],
                comics : [
                    {
                        id: 1,
                        title: 'Terms Of Use',
                        visible: true
                    },
                    {
                        id: 2,
                        title: 'Privacy policy (New)',
                        visible: true
                    },
                    {
                        id: 3,
                        title: 'Ad Choices',
                        visible: true
                    },
                    {
                        id: 4,
                        title: 'Advertising',
                        visible: true
                    },
                    {
                        id: 5,
                        title: 'Jobs',
                        visible: true,
                    },
                    {
                        id: 6,
                        title: 'Subscriptions',
                        visible: true,
                    },
                    {
                        id: 7,
                        title: 'Talent Workshops',
                        visible: true,
                    },
                    {
                        id: 8,
                        title: 'CPSC Certificates',
                        visible: true,
                    },
                    {
                        id: 9,
                        title: 'Ratings',
                        visible: true,
                    },
                    {
                        id: 10,
                        title: 'Shop Help',
                        visible: true,
                    },
                    {
                        id: 11,
                        title: 'Contact Us',
                        visible: true,
                    },
                ],
                sites : [
                    {
                        id: 1,
                        title: 'DC',
                        visible: true
                    },
                    {
                        id: 2,
                        title: 'MAD Magazine',
                        visible: true
                    },
                    {
                        id: 3,
                        title: 'DC Kids',
                        visible: true
                    },
                    {
                        id: 4,
                        title: 'DC Universe',
                        visible: true
                    },
                    {
                        id: 5,
                        title: 'DC Power Visa',
                        visible: true,
                    },
                ],
                contacts : [
                    {
                        id: 1,
                        image: 'img/footer-facebook.png',
                        visible: true
                    },
                    {
                        id: 2,
                        image: 'img/footer-pinterest.png',
                        visible: true
                    },
                    {
                        id: 3,
                        image: 'img/footer-twitter.png',
                        visible: true
                    },
                    {
                        id: 4,
                        image: 'img/footer-youtube.png',
                        visible: true
                    },
                    {
                        id: 5,
                        image: 'img/footer-periscope.png',
                        visible: true,
                    },
                ]
            }
        }
    }
</script>

<template> 

<footer>
   <section class="azzurra">
    <div>
        <ul >            
            <li  v-for="index in options" :key="index.id">
                <img :src="index.image" alt="">
                {{ index.title }}
            </li>
        </ul>
    </div>
   </section>
   <section class="info">
    <div>
        <ul>           
            <h1>DC COMICS</h1> 
            <li  v-for="index in dcComics" :key="index.id">
                {{ index.title }}
            </li>
            <h1>SHOP</h1>
            <li  v-for="index in shop" :key="index.id">
                {{ index.title }}
            </li>
        </ul>
        <ul>           
            <h1>DC</h1> 
            <li  v-for="index in comics" :key="index.id">
                {{ index.title }}
            </li>
        </ul>
        <ul>           
            <h1>SITES</h1> 
            <li  v-for="index in sites" :key="index.id">
                {{ index.title }}
            </li>
        </ul>
    </div>
   </section>
   <section class="follow">
        <div>
            <button>SIGN-UP NOW!</button>
            <ul>
                <h1>FOLLOW US </h1>
                <li  v-for="index in contacts" :key="index.id">
                    <img :src="index.image" alt="">
                </li>
            </ul>
        </div>
   </section>
</footer>
</template>

<style lang="scss" scoped> 
    @use '../styles/general.scss' as *;

    section.azzurra{
        background-color: #0282f9;

        div{
            width: 70%;
            margin: 0 auto;
            padding: 2rem 0rem;
            color:white;
        }

        ul{
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin: 0;
            padding: 0;

            li{
               display: flex;
               align-items: center;              
            }
        }

        img{
            width: 40px;
            padding-right: 1rem;
        }
    }

    section.info{
        background-image: url(/img/footer-bg.jpg);
        margin: 0;
      

        div{
            width: 70%;
            margin: 0 auto;
            padding: 1.5rem 0rem;
            display: flex;
        }

        ul{
            margin: 0;
            padding-right: 1.5rem;

            h1{
                color: white;
                font-size: 15px;
                margin: 0;
                padding: 1rem 0rem 0.7rem;
            }

            li{
                color:gray;
                font-size: 12px;
                padding-top: 0.5rem;
            }
        }

    }
    section.follow{
            background-color: #303030;

    
            div{
                width: 70%;
                margin: 0 auto;
                padding: 0.5rem 0rem;
                display: flex;
                justify-content: space-between;

                button{
                    background-color: #303030;
                    border-color: #0282f9;
                    color: white;
                }

                ul{
                    display: flex;

                    li{
                        padding-right: 1rem;
                    }

                    h1{
                        color: #0282f9;
                        font-size: 15px;
                        padding-right: 1rem;
                    }
                }
            }
    }
</style>
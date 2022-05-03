<template>
    <header>
        <div class="container">
            <nav>
                <div class="row align-items-center py-3">
                    <NavLogo/>
                    <div class="item-nav col-8">
                        <a class="text-uppercase text-decoration-none px-2 py-2 text-end active" href="#" v-for="({title}, index) in DcComics" :key="index">{{title}}</a>
                    </div>
                    <!-- /.item-nav -->
                </div>
                <!-- /.row -->
            </nav>
        </div>
    <!-- /.container -->
    </header>
</template>

<script>

import NavLogo from '@/components/NavLogoComponent'


export default {
    name: 'HeaderComponent',
    components: {
        NavLogo
    },
    data() {
        return {
        DcComics: [
            {
            title: 'Characters',
            },
            {
            title: 'Comics',
            },
            {
            title: 'Movies',
            },
            {
            title: 'Tv',
            },
            {
            title: 'Games',
            },
            {
            title: 'Collectibles',
            },
            {
            title: 'Videos',
            },
            {
            title: 'Fans',
            },
            {
            title: 'News',
            },
            {
            title: 'Shop',
            }
        ]
        };
    }
}
</script>

<style lang="scss" scoped>
    header  {
    text-align: center;
     nav {
         .item-nav{
             height: 100%;
         }

        a {
            height: 100%;
            color: #333;
            font-size: 14px;
            font-weight: 600;

            &.active:first-child {
                border-bottom: 3px solid blue;
            }
            &:hover {
                background-color: rgb(167, 184, 240) ;
            }
        } 
    }
}
</style>
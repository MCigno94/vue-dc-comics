<template>
  <footer class="text-white">
        <div class="footer_top">
            <div class="container d-flex">
                <div class="row w-100">
                    <div class="col-4">
                        <div class="row row-cols-3">
                            <div class="cols">
                                <h3>Dc comics</h3>
                                <ul class="text-secondary">
                                    <li v-for="({title}, index) in DcComics" :key="index">{{title}}</li>
                                </ul>
                            </div>
                            <!-- /.cols -->
                            <div class="cols">
                                <h3>DC</h3>
                                <ul class="text-secondary">
                                    <li>Lorem.</li>
                                    <li>ipsum.</li>
                                    <li>dolor.</li>
                                    <li>sit.</li>
                                    <li>amet.</li>
                                    <li>Lorem.</li>
                                    <li>ipsum.</li>
                                    <li>dolor.</li>
                                    <li>sit.</li>
                                    <li>amet.</li>
                                    <li>amet.</li>
                                </ul>
                            </div>
                            <!-- /.cols -->
                            <div class="cols">
                                <h3>Sites</h3>
                                <ul class="text-secondary">
                                    <li>Lorem.</li>
                                    <li>ipsum.</li>
                                    <li>dolor.</li>
                                    <li>sit.</li>
                                    <li>amet.</li>
                                </ul>
                            </div>
                            <!-- /.cols -->
                            <div class="cols">
                                <h3>Shop</h3>
                                <ul class="text-secondary">
                                    <li>Lorem.</li>
                                    <li>ipsum.</li>
                                </ul>
                            </div>
                            <!-- /.cols -->
                        </div>
                        <!-- /.row -->
                    </div>
                    <!-- /.col-4 -->    
                    <div class="col-3"></div>
                    <!-- /.col-3 -->        
                    <div class="logo_dc col-5 h-100">
                    <!-- <img src="@/assets/img/dc-logo-bg.png" alt="" class="logo_dc"> -->
                    </div>
                    <!-- /.col-4 -->
                </div>
                <!-- /.row -->
            </div>
            <!-- /.container -->
        </div>
        <!-- /.footer_top -->
        <div class="footer_bottom bg-dark">
            <div class="container d-flex justify-content-between align-items-center py-4">
                <div class="btn text-uppercase text-white border border-primary">
                    sign-up now!
                </div>
                <!-- /.btn -->
                <div class="social text-primary fw-bold">
                    <span class="text-uppercase px-2"> Follow Us</span>
                    <span class="icon_social">
                        <img src="@/assets/img/footer-facebook.png" alt="">
                        <img src="@/assets/img/footer-periscope.png" alt="">
                        <img src="@/assets/img/footer-pinterest.png" alt="">
                        <img src="@/assets/img/footer-twitter.png" alt="">
                        <img src="@/assets/img/footer-youtube.png" alt="">
                    </span>
                    <!-- /.icon_social -->
                </div>
                <!-- /.social -->
            </div>
            <!-- /.container -->
        </div>
        <!-- /.footer_bottom -->
  </footer>
</template>

<script>

export default {
  name: "FooterComponent",
  components :{

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
        ]
        };
    }
};
</script>

<style lang="scss" scoped>
footer {
    .footer_top{
        background-image: url('@/assets/img/footer-bg.jpg');
        .container {
            .row {
                .col-4{
                    padding-top: 2rem;
                }
            }
            .logo_dc {
                background-image: url('@/assets/img/dc-logo-bg.png');
                background-position: center;
                background-repeat: no-repeat;
                background-size: cover;
            }
            h3 {
                font-size: 14px;
                margin-bottom: 1rem;
                text-transform: uppercase;
            }
            ul {
                padding: 0;
                list-style: none;
                li {
                    font-size: 14px;
                }
            }
        }
    }
    .footer_bottom {
        .icon_social{
            img {
                padding: 0 0.25rem;
            }
        }
    }
}
</style>
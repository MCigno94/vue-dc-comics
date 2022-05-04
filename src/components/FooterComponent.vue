<template>
  <footer class="text-white">
        <div class="footer_top">
            <div class="container d-flex">
                <div class="row w-100">
                    <div class="col-4">
                        <div class="row row-cols-3">
                            <div class="cols">
                            <h3>Dc comics</h3>
                            <ul>
                                <li v-for="({title}, index) in DcComics" :key="index">{{title}}</li>
                            </ul>
                            </div>
                            <!-- /.cols -->
                            <div class="cols">
                            <h3>DC</h3>
                            <ul>
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
                            <ul>
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
                            <ul>
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
        <div class="footer_bottom"></div>
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
    background-image: url('@/assets/img/footer-bg.jpg');
    .container {
        .logo_dc {
            background-image: url('@/assets/img/dc-logo-bg.png');
            background-position: center;
            background-repeat: no-repeat;
            background-size: cover;
        }
        h3 {
            font-size: 1rem;
            margin-bottom: 1rem;
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
</style>
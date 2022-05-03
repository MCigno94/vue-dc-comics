<template>
        <main class="text-white">
        <section class="jumbotrone">
          <div class="container">
              <p class="text-white">Contenuto Qui</p>
          </div>
          <!-- /.container -->
        </section>
        <!-- /.jumbotrone -->
        <section class="footer_main">
          <div class="container">
            <div class="row row-cols-5">
              <div class="cols d-flex align-items-center" v-for="({titolo}, index) in itemFooter" :key="index">
                  <img class="image img-fluid" src="@/assets/img/buy-comics-digital-comics.png" :alt="titolo" />
                  <div class="description text-uppercase px-3">{{titolo}}</div>
                  <!-- /.description -->
              </div>
              <!-- /.cols -->
            </div>
            <!-- /.row -->
          </div>
          <!-- /.container -->

        </section>
        <!-- /.footer_main -->
    </main>
</template>

<script>

export default {
    name: 'MainComponent',
    components: {
        
    },
    data() {
        return {
            itemFooter: [
                {
                    src: "@/assets/img/buy-comics-digital-comics.png",
                    titolo: "Digital Comics"
                },
                {
                    src: "@/assets/img/buy-comics-merchandise.png",
                    titolo: "DC Merchandise"
                },
                {
                    src: "@/assets/img/buy-comics-shop-locator.png",
                    titolo: "Subscription"
                },
                {
                    src: "@/assets/img/buy-comics-subscriptions.png",
                    titolo: "Comic Shop Locator"
                },
                {
                    src: "@/assets/img/buy-dc-power-visa.svg",
                    titolo: "DC Pover Visa"
                },

            ]
        };
    }
}
</script>

<style lang="scss" scoped>
    .jumbotrone {
    background-color: black;
    height: 130px;
    }

    .footer_main {
        background-color: blue;
        z-index: 10;
        .container {
            .row {
                padding: 3rem 1.5rem;
                
                .image{
                    
                        height: 50px;
                    
                }
                .description{
                    font-size: 14px;
                }
            }
        }
    }
</style>
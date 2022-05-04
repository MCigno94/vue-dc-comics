<template>
        <main class="text-white ">
        <SectionJumbo />
        <SectionCard />
        <section class="banner bg-primary">
          <div class="container">
            <div class="row row-cols-5">
              <div class="cols d-flex align-items-center" v-for="({titolo, src}, index) in itemBanner" :key="index">
                  <img class="image img-fluid" :src="src" :alt="titolo" />
                  <div class="description text-uppercase px-3">{{titolo}}</div>
                  <!-- /.description -->
              </div>
              <!-- /.cols -->
            </div>
            <!-- /.row -->
          </div>
          <!-- /.container -->

        </section>
        <!-- /.banner -->
    </main>
</template>

<script>
import SectionCard from '@/components/SectionCardComponent';
import SectionJumbo from '@/components/SectionJumboComponent';


export default {
    name: 'MainComponent',
    components: {
        SectionCard,
        SectionJumbo
    },
    data() {
        return {
            itemBanner: [
                {   
                    id: 1,
                    src: require("@/assets/img/buy-comics-digital-comics.png"),
                    titolo: "Digital Comics"
                },
                {   
                    id: 2,
                    src: require("@/assets/img/buy-comics-merchandise.png"),
                    titolo: "DC Merchandise"
                },
                {   
                    id: 3,
                    src: require("@/assets/img/buy-comics-shop-locator.png"),
                    titolo: "Subscription"
                },
                {
                    id: 4,
                    src: require("@/assets/img/buy-comics-subscriptions.png"),
                    titolo: "Comic Shop Locator"
                },
                {
                    id: 5,
                    src: require("@/assets/img/buy-dc-power-visa.svg"),
                    titolo: "DC Pover Visa"
                },

            ]
        };
    }
}
</script>

<style lang="scss" scoped>

    .banner {
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
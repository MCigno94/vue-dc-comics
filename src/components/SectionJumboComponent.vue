<template>

    <section class="jumbotrone">
        <img src="@/assets/img/jumbotron.jpg" alt="jumbo-image">
    </section>
    <!-- /.jumbotrone -->
  
</template>

<script>
export default {
    name: "SectionJumbo"
}
</script>

<style lang="scss" scoped>
.jumbotrone {
    img {
    max-width: 100%;
    width: 100%;
    object-fit: cover;
    object-position: top;
    height: 530px;
    display: block;
    }
}

</style>
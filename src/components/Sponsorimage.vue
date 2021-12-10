<template>
  <section>
        <div class="container">
            <div class="container-image" 
                v-for="(element, i) in listSponsor" :key="`image-${i}`">

                <img :src="require(`@/assets/img/${element}.png`)" alt="">
            </div>
        </div>
  </section>
</template>

<script>
export default {
    name: 'Sponsorimage',
    props: {
        listSponsor: Array,
    }
}
</script>

<style lang="scss" scoped>
@import '@/style/variables';
section{
    margin-bottom: 50px;
}
.container{
    display:flex;
    justify-content: center;
    align-items: center;

}

img{
    width: 120px;
    padding: 0 20px;
    filter: grayscale(100%) opacity(30%);
}

</style>
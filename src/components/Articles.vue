<template>
  <section>
        <div class="container">

            <div class="title-section">

                <span class="col-gray text-spacing uppercase intro">
                    blog update
                </span>

                <h2 class="font-title">
                    Interesting 
                    <span class="text-other-color font-title">articles updated</span>
                    daily
                </h2>
            </div>

            <div class="list-card">


                <div class="created-card" 
                    v-for="(element, i) in listArticles" :key="`element-${i}`">

                    <CardCourses :url="element.poster"
                                    :date="element.date"
                                    :title="element.title"
                                    :description="element.description" />

                    <!-- <div class="card">

                        <img src="@/assets/img/motivation-course-06-480x298.jpg" alt="poster">

                        <div class="text">

                            <span class="price text-other-color">
                                <span>$30</span>.00
                            </span>

                            <p class="description">
                                How to be Successful: Create A Growth Mindset For Succes
                            </p>

                            <div class="statistic">
                                <span class="lesson">
                                    <i class="far fa-file-alt"></i>
                                    3 lessons
                                </span>

                                <span class="people">
                                    <i class="far fa-user"></i>
                                    50 students
                                </span>
                            </div>
                        </div>
                    </div> -->
                </div>

            </div>


            <div class="button-section">
                <span class="uppercase text-spacing text-other-color">
                    view all post
                </span>
            </div>

        </div>
  </section>
</template>

<script>
import CardCourses from "@/components/CardCourses.vue" 

export default {
    name: 'Articles',

    props: {
        listArticles: Array,
    },

    components: {
        CardCourses,
    },
}

</script>

<style lang="scss" scoped>
@import '@/style/variables';

section{
    margin-bottom: 50px;
}

.title-section{
    margin-bottom: 30px;

    .intro{
        font-size: 14px;
    }

    h2{
        font-size: 32px;
    }
}

.list-card{
    display: flex;
    flex-wrap: wrap;
    margin-bottom: 30px;
}

.created-card{
    width: calc(100% / 4);
    padding: 10px;
}

.button-section{
    text-align: center;

    span{

        font-size: 14px;
        font-weight: bold;
        border-bottom: 2px solid currentColor;
        cursor: pointer;

        &:hover{
            color: $color-list-nav;
        }
    }
}

</style>
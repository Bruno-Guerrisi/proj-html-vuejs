<template>
  <section>
        <div class="container">

            <div class="title-section">

                <span class="col-gray text-spacing uppercase intro">
                    begin your journay at maxcoach
                </span>

                <h2 class="font-title">
                    Latest <span class="text-other-color font-title">Online Courses</span>
                </h2>
            </div>

            <div class="list-card">


                <div class="created-card" 
                    v-for="(element, i) in listCourses" :key="`element-${i}`">

                    <CardCourses :url="element.poster"
                                    :dollars="element.dollars"
                                    :cents="element.cents"
                                    :description="element.description"
                                    :lesson="element.lesson"
                                    :students="element.students" />

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

                <button class="hover-button">
                    Get Started For Free

                    <i class="fas fa-long-arrow-alt-right"></i>
                </button>
            </div>

        </div>
  </section>
</template>

<script>
import CardCourses from "@/components/CardCourses.vue" 

export default {
    name: 'Courses',

    props: {
        listCourses: Array,
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
    text-align: center;
    margin-bottom: 30px;

    .intro{
        font-size: 14px;
    }

    h2{
        font-size: 38px;
    }
}

.list-card{
    display: flex;
    flex-wrap: wrap;
    margin-bottom: 30px;
}

.created-card{
    width: calc(100% / 3);
    padding: 10px;
}

.button-section{
    text-align: center;

    button{
        width: 25%;
        min-width: 15%;
        background-color: $alternativ-text-bt-price;
        color: $color-white;
        border: 0;
        padding: 15px;
        border-radius: 5px;
        font-weight: bold;
    }
}

</style>
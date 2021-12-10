<template>
    <div class="card">

        <img :src="url" alt="poster">

        <div class="text">

            <span class="price text-other-color">
                <span>{{dollars}}</span>.{{cents}}
            </span>

            <p class="description">
                {{description}}
            </p>

            <div class="statistic">
                <span class="lesson">
                    <i class="far fa-file-alt"></i>
                    {{lesson}} lessons
                </span>

                <span class="people">
                    <i class="far fa-user"></i>
                    {{students}} students
                </span>
            </div>
        </div>
    </div>
</template>

<script>

export default {
    name: 'CardCourses',

    props: {
        url: String,
        dollars: String,
        cents: String,
        description: String,
        lesson: Number,
        students: Number,
    },
}
</script>

<style lang="scss" scoped>
@import '@/style/variables';

.card{
    // background-color: rgb(255, 255, 255);
    border-radius: 5px;
    cursor: pointer;
    transition: 0.2s;

    &:hover{
        box-shadow: 5px 10px 16px 2px rgba(0,0,0,0.38);
    }

    .text{
        padding: 5px 15px 20px;
    }

    .price{
        font-size: 14px;
        display: block;
        margin-bottom: 10px;
        font-weight: bold;

        span{
            font-size: 22px;
        }
    }

    .description{
        font-weight: bold;
        font-size: 18px;
        margin-bottom: 10px;
    }

    .statistic{
        color: $color-gray;
        font-size: 14px;

        .lesson{
            margin-right: 20px;
        }
    }

}

</style>
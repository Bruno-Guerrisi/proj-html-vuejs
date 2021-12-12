<template>
    <div class="card">

        <img :src="url" alt="poster">

        <div class="text">

            <span v-if="dollars != null && cents != null" 
                    class="price text-other-color">
                <span>${{dollars}}</span>.{{cents}}
            </span>

            <span v-if="date != null" class="date">
                <i class="far fa-calendar"></i>
                {{date}}
            </span>

            <p class="title">
                {{title}}
            </p>

            <div  v-if="lesson != null && students != null"
                    class="statistic">
                <span class="lesson">
                    <i class="far fa-file-alt"></i>
                    {{lesson}} lessons
                </span>

                <span class="people">
                    <i class="far fa-user"></i>
                    {{students}} students
                </span>
            </div>

            <div v-if="description != null" class="description">
                <p>
                    {{description}}
                </p>
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
        title: String,
        lesson: Number,
        students: Number,

        date: String,
        description: String,
    },
}
</script>

<style lang="scss" scoped>
@import '@/style/variables';

.card{
    height: 100%;
    border-radius: 5px;
    overflow: hidden;
    cursor: pointer;
    transition: 0.2s;

    &:hover{
        box-shadow: 5px 10px 16px 2px rgba(0,0,0,0.38);
    }

    .text{
        padding: 5px 15px 20px;
    }

    .title{
        font-weight: bold;
        font-size: 18px;
        margin-bottom: 10px;
    }


    /* courses scss */

    .price{
        font-size: 14px;
        display: block;
        margin-bottom: 10px;
        font-weight: bold;

        span{
            font-size: 22px;
        }
    }

    .statistic{
        color: $color-gray;
        font-size: 14px;

        .lesson{
            margin-right: 20px;
        }
    }


    /* articles scss */

    .date{
        color: $color-gray;
        display: block;
        padding-top: 8px;
        font-size: 14px;
        margin-bottom: 8px;

        i{
            margin-right: 5px;
        }
    }

    .description{
        padding-top: 3px;
        color: $color-gray;
        font-size: 14px;
    }

}

</style>
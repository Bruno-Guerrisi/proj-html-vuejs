<template>
    <section>

        <div class="row">

            <div class="col-left col">

                <span class="text-spacing uppercase text-other-color info">
                    real stories
                </span>

                <p>
                    I am free to learn at my own pace, follow my own schedule and choose the subject i want to learn from the syllabus. Great study portal for people like me.
                </p>

                <div class="people-stories">
                    <img src="@/assets/img/testimonial-avata-02.jpg" alt="people stories">

                    <span class="name">Mina Hollance</span>

                    <span class="work">/ Freelanceer</span>
                </div>

            </div>

            <div class="col-right col">
                <img src="@/assets/img/home-movation-testimonial-image.jpg" alt="poster">
            </div>

            <div class="central-button">

                <i class="fas fa-sort-up"></i>

                <span> 1 / 4</span>

                <i class="fas fa-sort-down"></i>
            </div>
        </div>
    </section>
</template>

<script>
export default {
name: 'Stories',
}
</script>

<style lang="scss" scoped>
@import '@/style/variables';

section{
    margin-bottom: 50px;
}

.row{
    width: 100%;
    height: 490px;
    display: flex;
    overflow: hidden;
    position: relative;

    .central-button{
        width: 60px;
        height: 60px;
        border-radius: 50%;
        background-color: white;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);

        span{
            margin: 1px 0;
            font-size: 12px;
        }

        i{
            cursor: pointer;
        }
    }

    .col{
        width: 50%;
    }

    .col-left{
        height: 100%;
        position: relative;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;

        span.info{
            display: block;
            margin-bottom: 30px;
            font-size: 12px;
        }

        p{
            max-width: 52%;
            text-align: center;
            font-size: 18px;
            line-height: 30px;
            margin-bottom: 20px;
        }

        .people-stories{
            text-align: center;

            img{
                width: 60px;
                height: 60px;
                border-radius: 50%;
                margin-bottom: 10px;
            }

            span{
                display: block;

                &:first-of-type{
                    margin-bottom: 10px;
                }

                &:last-child{
                    color: $color-gray;
                    font-size: 12px;
                }
            }
        }

        &::before{
            content: "";
            position: absolute;
            width: 100%;
            height: 100%;
            background-color: #eaeaea;
            z-index: -1;
            background-image: url('../assets/img/background-pattern-wavify.png');
        }
    }
    
    .col-right{

        img{
            object-fit: cover;
            height: 100%;
        }
    }
}

</style>
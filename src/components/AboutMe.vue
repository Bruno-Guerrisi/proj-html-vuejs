<template>
    <section>
        <div class="container">

            <span class="uppercase title-section text-spacing">about me</span>

            <div class="row-left row">

                <div class="col-left col">
                    <h3 class="font-title">
                        How to Be an Alpha Male: The 15 Habits of True Alphas
                    </h3>
                </div>

                <div class="col-right col">
                    <p class="question">
                        Want to learn how to be <span class="text-other-color">an alpha male</span>? How to be more masculine? <br>
                        How to be the man you've always wanted to be?
                    </p>

                    <p class="answers">
                        Your goal is to show the consistency of business, core values, and custorer care Punctuality, responsibility, individuality, accuracy, enthusiast you have to clearly explain how these qualities are applicable to your work. And the important thing is you do love what you do.
                    </p>
                </div>
            </div>

            <div class="row-right row">

                <div class="col-left col">
                    <img src="@/assets/img/home-movation-video-poster-670x450.jpg" alt="video youtube">

                    <img class="logo-youtube" src="@/assets/img/icon-youtube-play.png" alt="youtube logo">
                </div>

                <div class="col-right col">

                    <p class="font-title">
                        "Every morning you have two choices: continue to sleep with your dreams, or wake up and chase them."
                    </p>

                    <img src="@/assets/img/home-movation-shape-01.png" alt="home motivation logo">

                    <span class="author">Kaixa Stark</span>

                    <span class="uppercase text-spacing">wingman</span>
                </div>

            </div>
        </div>
    </section>
</template>

<script>
export default {
name: 'AboutMe',
}
</script>

<style lang="scss" scoped>
@import '@/style/variables';

section{
    margin-bottom: 70px;
}

.title-section{
    color: $alternativ-text-bt-price;
    font-size: 14px;
    margin-bottom: 20px;
    display: inline-block;
}

.row{
    display: flex;
}

.row-left{

    margin-bottom: 60px;

    .col-left{
        width: 45%;
        h3{
            max-width: 70%;
            font-size: 34px;
        }
    }

    .col-right{
        width: 55%;

        .question{
            font-size: 16px;
            margin-bottom: 10px;
            line-height: 30px;
            font-weight: bold;
        }

        .answers{
            color: $color-gray;
            font-size: 16px;
        }
    }
}

.row-right{
    align-items: center;

    .col-left{
        width: 50%;
        position: relative;
        
        img{
            border-radius: 10px;
            cursor: pointer;
        }

        .logo-youtube{
            position: absolute;
            top: 50%;
            left: 50%;
            width: 80px;
            transform: translate(-50%, -50%);
        }

    }

    .col-right{
        width: 50%;
        padding: 0 13%;
        display: flex;
        flex-direction: column;

        p.font-title{
            font-size: 22px;
            margin-bottom: 40px;
        }

        img{
            width: 30px;
            margin-bottom: 10px;
        }

        .author{
            font-weight: bold;
            font-size: 18px;
            margin-bottom: 5px;
        }
        
        span:last-child{
            font-size: 12px;
            color: $color-gray;
        }
    }
}

</style>
<template>
    <section>
            <div class="container">

                <div class="components">

                    <div class="left-components">
                        
                        <span class="uppercase">i'm wingman</span>

                        <h2 class="font-title">Peace On Earth A Wounderful Wish But No Way</h2>

                        <p>
                            Secces isn't overnight. It's when everyday you get a little better than the day before. It all adds up.
                        </p>

                        <button class="hover-button">
                            Get Started For Free

                            <i class="fas fa-long-arrow-alt-right"></i>
                        </button>
                    </div>
                </div>

                <div class="components">

                    <div class="right-components">
                        
                        <div class="image-one">
                            <img src="@/assets/img/home-movation-shape-face.png" alt="">
                        </div>

                        <div class="image-two">
                            <img src="@/assets/img/home-movation-hero-image.png" alt="">
                        </div>
                    </div>
                </div>
            </div>
    </section>
</template>

<script>
export default {
name: 'MainIntro',
}
</script>

<style lang="scss" scoped>
@import '@/style/variables';

section{
    background-image: url('../assets/img/background-pattern-wavify.png');
    width: 100%;
    height: 520px;
    position: relative;

    &::before{
        content: '';
        position: absolute;
        width: 100%;
        height: 100%;
        background-color: #eaeaea;
        z-index: -1;
    }
}
.container{
    padding-top: 80px;
    height: 100%;
    display: flex;
}

.components{
    width: calc(100% / 2);
    height: 100%;
}

.left-components{
    display: flex;
    flex-direction: column;
    justify-content: center;
    max-width: 60%;
    height: 100%;

    span{
        font-size: 14px;
        letter-spacing: 1px;
        margin-bottom: 10px;
        color: $title-color;
    }

    h2{
        font-size: 40px;
        margin-bottom: 10px;
        color: $title-color;
    }

    p{
        font-size: 14px;
        color: $color-gray;
        margin-bottom: 20px;
        line-height: 25px;
    }

    button{
        width: 65%;
        min-width: 40%;
        background-color: $alternativ-text-bt-price;
        color: $color-white;
        border: 0;
        padding: 15px;
        border-radius: 5px;
    }
}

.right-components{
    position: relative;
    height: 100%;
    overflow: hidden;

    .image-one{
        position: absolute;
        bottom: 0;
        left: 50%;
        transform: translateX(-50%);
        width: 70%;
    }

    .image-two{
        position: absolute;
        bottom: -5px;
        left: 40%;
        transform: translateX(-50%);
        width: 65%;
    }
}

</style>
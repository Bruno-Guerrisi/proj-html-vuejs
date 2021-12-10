<template>
  <section>
      <div class="container">

        <div class="col-left">
            <span class="uppercase text-spacing intro">
                book store online
            </span>

            <h2 class="font-title">
                Be Alpha With <span class="font-title text-other-color">Wingman's Book</span>
            </h2>

            <ul>
                <li>
                    <i class="fas fa-check text-other-color"></i>
                    Help you understand yourself better
                </li>

                <li>
                    <i class="fas fa-check text-other-color"></i>
                    Revealing mature tips
                </li>

                <li>
                    <i class="fas fa-check text-other-color"></i>
                    Give the right advice
                </li>

                <li>
                    <i class="fas fa-check text-other-color"></i>
                    Fascinating example of alpha man
                </li>
            </ul>

            <button class="hover-button">
                Get Free Book

                <i class="fas fa-long-arrow-alt-right"></i>
            </button>
        </div>

        <div class="col-right">

            <div class="book">

                <div class="container-image">

                    <img src="@/assets/img/product-book-11-400x400.jpg" alt="">

                    <div class="container-box">

                        <div class="box">
                            <i class="fas fa-search"></i>
                        </div>
                        <div class="box">
                            <i class="fas fa-cart-arrow-down"></i>
                        </div>
                        <div class="box">
                            <i class="far fa-heart"></i>
                        </div>
                        <div class="box">
                            <i class="fas fa-signal"></i>
                        </div>
                    </div>
                </div>

                <span class="title">Alpha man by Maxcoach</span>

                <span class="price text-other-color">
                    <span>$29</span>.00
                </span>
            </div>

            <div class="book">

                <div class="container-image">

                    <img src="@/assets/img/product-book-10-400x400.jpg" alt="">

                    <div class="container-box">

                        <div class="box">
                            <i class="fas fa-search"></i>
                        </div>
                        <div class="box">
                            <i class="fas fa-cart-arrow-down"></i>
                        </div>
                        <div class="box">
                            <i class="far fa-heart"></i>
                        </div>
                        <div class="box">
                            <i class="fas fa-signal"></i>
                        </div>
                    </div>
                </div>

                <span class="title">Alpha man by Maxcoach</span>

                <span class="price text-other-color">
                    <span>$29</span>.00
                </span>
            </div>
        </div>

      </div>
  </section>
</template>

<script>
export default {
name: 'Bookstore',
}
</script>

<style lang="scss" scoped>
@import '@/style/variables';

section{
    margin-bottom: 50px;
}

.container{
    display: flex;
}

.col-left{
    width: 35% ;

    .intro{
        font-size: 14px;
        margin-bottom: 20px;
        display: block;
    }

    h2{
        font-size: 32px;
        margin-bottom: 25px;
    }

    ul{
        margin-bottom: 35px;

        li{
            list-style: none;
            margin-bottom: 8px;
        }
    }
}

.col-right{
    width: 65%;
    height: 100%;
    display: flex;

    .book{
        height: 100%;
        width: calc(100% / 2);
        text-align: center;
        padding: 10px;

        img{
            height: 300px;
            object-fit: cover;
        }

        .title{
            font-weight: bold;
            margin-bottom: 5px;
            display: block;
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
    }

.container-image{
    position: relative;
    cursor: pointer;

    &:hover .container-box .box{
        opacity: 1;
    }

    .container-box{
        position: absolute;
        top: 48%;
        transform: translateY(-50%);
        right: 20px;

        .box{
            width: 50px;
            height: 50px;
            background-color: white;
            border-radius: 50%;
            display: flex;
            justify-content: center;
            align-items: center;
            margin: 10px 0;
            box-shadow: 5px 10px 16px 2px rgba(0,0,0,0.38);
            opacity: 0;
            transition: 0.2s;

            &:hover {
                background-color: $color-list-nav;
                color: white;
            }
        }
    }
}

}


button{
    width: 50%;
    min-width: 40%;
    background-color: $alternativ-text-bt-price;
    color: $color-white;
    border: 0;
    padding: 15px;
    border-radius: 5px;
    font-weight: bold;
}

</style>
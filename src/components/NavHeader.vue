<template>
  <section>

    <div class="container">

        <!-- logo -->
        <a href="#" class="logo">
            <img src="@/assets/img/dark-logo.png" alt="logo">
        </a>

        <!-- navbar -->
        <ul>
            <li v-for="(element, i) in listNav" :key="`element-${i}`"
                class="list-nav">
                <span>{{element}}</span>

                <i class="fas fa-chevron-down"></i>
            </li>
        </ul>

        <!-- link social -->

        <ul>

            <li class="icon-social">
                <a href="#">
                    <i class="fab fa-twitter"></i>
                </a>
            </li>

            <li class="icon-social">
                <a href="#">
                    <i class="fab fa-facebook-f"></i>
                </a>
            </li>

            <li class="icon-social">
                <a href="#">
                    <i class="fab fa-linkedin"></i>
                </a>
            </li>

            <li class="icon-social">
                <a href="#">
                    <i class="fab fa-instagram"></i>
                </a>
            </li>
        </ul>
    
    </div>

  </section>
</template>

<script>
export default {
name: 'NavHeader',

data(){
    return{
        listNav: [
            'Home',
            'Pages',
            'Courses',
            'Features',
            'Blog',
            'Shop',
        ]
    }
}


}
</script>

<style lang="scss" scoped>
@import '@/style/variables';

section{
    height: 60px;
    display: flex;
    align-items: center;
}

.container{
    display: flex;
    align-items: center;
    justify-content: space-between;
    width: 100%;
}

a.logo{
    display: block;
    width: 150px;
    height: 100%;
}

ul{
    display: flex;
    list-style: none;

    .list-nav{
        margin: 0 15px;

        span{
            color: $color-list-nav;
            cursor: pointer;
        }

        i{
            margin-left: 5px;
            font-size: 12px;
            cursor: pointer;
        }
    }

    .icon-social{
        margin: 0 10px;

        a{
            i{
                font-size: 18px;
                color: $text-color;
            }
        }
    }
}

</style>
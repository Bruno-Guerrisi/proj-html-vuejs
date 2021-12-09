<template>
    <section>

        <div class="container">

            <ul>
                <li  v-for="(element, i) in listStatistic" :key="`element-${i}`">

                    <img src="@/assets/img/background-pattern-grid-line-06.png" alt="">
                    <span class="number">{{element.numberStatistic}}</span>
                    <span class="uppercase text">{{element.infoText}}</span>
                    <img v-if="i == listStatistic.length -1"
                        class="last-rotate"
                        src="@/assets/img/background-pattern-grid-line-06.png" alt="">
                </li>
            </ul>
        </div>
    </section>
</template>

<script>
export default {
    name: 'Statistics',

    data(){
        return{
            listStatistic: [
                {
                    numberStatistic: '1.926',
                    infoText: 'finisched session'
                },
                {
                    numberStatistic: '100%',
                    infoText: 'satisfaction rate'
                },
                {
                    numberStatistic: '3092+',
                    infoText: 'enrolled learners'
                },
                {
                    numberStatistic: '200',
                    infoText: 'online instructors'
                },
            ],
        }
    },
}
</script>

<style lang="scss" scoped>
@import '@/style/variables';

section{
    padding: 80px 0;
}

ul{
    display: flex;
}

li{
    list-style: none;
    display: flex;
    flex-direction: column;
    align-items: center;
    position: relative;
    width: calc(100% / 4);
    overflow: hidden;

    img{
        position: absolute;
        top: 0;
        left: 0;
        height: 200px;
    }

    .last-rotate{
        transform: rotate(180deg);
    }

    .number{
        margin-bottom: 10px;
        color: $alternativ-text-bt-price;
        font-size: 26px;
    }

    .text{
        letter-spacing: 1px;
        font-size: 14px;
        color: $title-color;
    }
}

</style>>

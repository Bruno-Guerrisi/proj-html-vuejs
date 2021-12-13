<template>
    <a class="button-up" href="#up">
        <i class="fas fa-long-arrow-alt-up"></i>
    </a>
</template>

<script>
export default {
    name: 'Returnup',
}
</script>

<style lang="scss" scoped>
@import '@/style/variables';

.button-up{
    width: 50px;
    height: 50px;
    position: fixed;
    right: 10px;
    bottom: 20px;
    padding: 7px;
    background-color: $alternativ-text-bt-price;
    border-radius: 50%;
    z-index: 10;
    display: flex;
    justify-content: center;
    align-items: center;
    cursor: pointer;
    text-decoration: none;
    animation: up-arrow 0.8s infinite  alternate;

    i{
        font-size: 18px;
        color: white;
    }
}

@keyframes up-arrow {
    from {
        transform: translateY(0);
    }
    to {
        transform: translateY(10px);
    }
}

</style>
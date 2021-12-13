<template>
    <div class="icon-container">
        <i class="fas fa-ruler-combined"></i>

        <i class="far fa-life-ring"></i>

        <i class="fas fa-book"></i>

        <i class="fas fa-cart-arrow-down"></i>
    </div>
</template>

<script>
export default {
name: 'Navright'
}
</script>

<style lang="scss" scoped>

.icon-container{
    position: fixed;
    right: 0%;
    bottom: 50%;
    transform: translateY(-50%);
    padding: 7px;
    background-color: white;
    border-top-left-radius: 5px;
    border-bottom-left-radius: 5px;
    z-index: 10;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    box-shadow: -3px 10px 19px -1px rgba(0,0,0,0.34);

    i{
        margin: 4px 0;
        cursor: pointer;
    }
}

</style>
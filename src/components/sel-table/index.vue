<template>  
    <div class="sel-table">
        <div class="sel-table__element"></div>
    </div>
</template>

<script>
export default {
    data() {
        return {

        }
    }
}
</script>

<style lang="scss" scoped>
    .sel-table{
        width:100px;
        height:100px;
        border:1px solid #f66;
        &__element{
            width:50px;
            height:50px;
            background:#f66;
        }
    }
</style>

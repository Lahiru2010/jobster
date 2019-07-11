<template>
    <div class="content">
        <Menu></Menu>
    </div>
</template>

<script>
import Menu from './Menu.vue'
export default {
    components:{
        Menu:Menu
    }

}
</script>

<style lang="scss">
.content{
    min-height: 1000px;
}
</style>

<template>
    <div class="sidebar">
        <div v-for="(item, idx) in items" :key="idx">
            {{ idx+1 }}. {{ item.row }}
        </div>
    </div>
</template>

<script>
export default {
    props: {
        items: {
            type: Array,
            default: () => []
        }
    }
}
</script>

<style lang="scss" scoped>
$sidebar-orange: #F5523B;
.sidebar {
    width: 250px;
    padding: 12px 18px;
    color: #fff;
    height: 100vh;
    position: fixed;
    z-index: 999;
    background: $sidebar-orange;
    border: 1px solid rebeccapurple;
}
</style>

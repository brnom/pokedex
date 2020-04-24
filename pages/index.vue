<template>
    <div class="container">
        Landing Page :)
        <logo class="logo" />
    </div>
</template>

<script>
import Logo from '@/static/logo.svg'
export default {
    components: {
        Logo
    }
}
</script>

<style lang="scss" scoped>
.container {
    // padding: 12px 18px;
    & > .logo {
        border: 1px solid red;
    }
}
</style>

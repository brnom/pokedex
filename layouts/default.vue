<template>
    <div>
        <sidebar :items="items" />
        <div class="main">
            <nuxt />
        </div>
    </div>
</template>

<script>
import Sidebar from '@/components/Sidebar'

export default {
    components: {
        Sidebar
    },
    data () {
        return {
            items: [{ row: 'All' }, { row: 'Fav' }, { row: 'Type' }]
        }
    }
}
</script>

<style>
html {
  font-family: 'Source Sans Pro', -apple-system, BlinkMacSystemFont, 'Segoe UI',
    Roboto, 'Helvetica Neue', Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
}

.main {
    border: 1px solid red;
    padding: 32px 40px;
}
</style>

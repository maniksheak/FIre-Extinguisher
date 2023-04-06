<template>
  <div>
    <h2> Hello i am route /products/id</h2>
    {{ products }}
  </div>
</template>

<script>
import { mapState } from 'vuex';
export default {
  computed: {
    ...mapState([
       'products'
    ])
  }
}
</script>

<style lang="scss" scoped></style>
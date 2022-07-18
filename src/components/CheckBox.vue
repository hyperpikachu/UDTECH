<template>
  <div class="q-pa-md">
    <div class="q-gutter-sm">

      <div class="checkbox">
        <q-checkbox left-label v-model="left" label="Label on Left" />
      </div>

    </div>
  </div>
</template>

<script>
import { ref } from 'vue'

export default {

  setup () {
    return {
      left: ref(true),
      right: ref(false),
      left2: ref(true),
      right2: ref(false)
    }
  }
}
</script>

<style lang="scss">
.checkbox {
    display: flex;
    position: relative;
    justify-content: center;
  }
</style>

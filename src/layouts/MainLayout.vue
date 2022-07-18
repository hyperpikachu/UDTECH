<template>
  <q-layout view="hHh lpR fFf">

    <q-header elevated class="bg-primary text-white" height-hint="98">
      <q-toolbar>
        <q-toolbar-title>
          <q-avatar>
            <img src="https://cdn.quasar.dev/logo-v2/svg/logo-mono-white.svg">
          </q-avatar>
          유디테크
        </q-toolbar-title>
         <q-tabs>
        <q-route-tab to="/page1" label="회사소개" />
        <q-route-tab to="/page2" label="사업소개" />
        <q-route-tab to="/page3" label="상품권" />
        <q-route-tab to="/page3" label="쇼핑" />
      </q-tabs>
      </q-toolbar>


    </q-header>

    <q-page-container>
      <router-view />
    </q-page-container>

    <q-footer elevated class="bg-grey-8 text-white">
      <q-toolbar>
        <q-toolbar-title>
          <q-avatar>
            <img src="https://cdn.quasar.dev/logo-v2/svg/logo-mono-white.svg">
          </q-avatar>
          <div>Title</div>
        </q-toolbar-title>
      </q-toolbar>
    </q-footer>

  </q-layout>
</template>

<script>
import { defineComponent, ref } from 'vue'
import EssentialLink from 'components/EssentialLink.vue'



export default defineComponent({
  name: 'MainLayout',

  components: {

  },

  setup () {

    return {

      }
    }
  }
)

</script>

<style scoped lang="scss">

.title {
  display: flex;
  font-size: 100px;
  font-weight: 700;
  color: aquamarine;
  position: relative;
  // background-color: red;
  // top: 20px;
  align-items: center;
  .messi {
    top: -10px;
    // background-color: blue;
  }
  .date {
    position: absolute;
    right: 30px;
    // background-color: black;
  }
}


</style>

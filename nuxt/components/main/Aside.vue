<template>
  <div class="aside-wrapper">
    <b-nav vertical>
      <b-nav-item>Проекты</b-nav-item>
      
      <b-nav-item>Должники</b-nav-item>
      
      <b-nav-item v-b-toggle.collapse-1 align-v="center">
        <span>Корреспонденция</span>
        <b-icon icon="chevron-right" style="font-size: 13px"></b-icon></b-nav-item>
      <b-collapse id="collapse-1" class="mt-2">
        <!-- <b-list-group>
          <b-list-group-item href="#">submenu</b-list-group-item>
          <b-list-group-item href="#">submenu</b-list-group-item>
          <b-list-group-item href="#" button>submenu</b-list-group-item>
          <b-list-group-item href="#" button>submenu</b-list-group-item>
        </b-list-group> -->
        
        <!-- <b-link href="#foo">Link</b-link>
        <b-link href="#foo">Link</b-link>
        <b-link href="#foo">Link</b-link>
        <b-link href="#foo">Link</b-link> -->

        <b-nav vertical class="ml-4">
          <b-nav-item>Входящие</b-nav-item>
          <b-nav-item>Исходящие</b-nav-item>
          <b-nav-item>Корреспонденты</b-nav-item>
        </b-nav>
      </b-collapse>

      <b-nav-item>Link</b-nav-item>

    </b-nav>
  </div>
  

</template>


<script>
import { BIcon, BIconChevronDown, BIconChevronRight } from 'bootstrap-vue'
export default {
  name: "Aside",
  components: {
    BIcon,
    BIconChevronDown,
    BIconChevronRight
  },

}
</script>


<style lang="css" scope>

  .aside-wrapper {
    height: calc(100vh + 60px);
    width: 200px;
    background-color: #1F2937;
    color: #9CA3AF;
  }

  .nav-link {
    /* align-items: center; */
    /* align-content: center; */
    /* text-align: center; */
    /* vertical-align: middle; */
  }
  
</style>
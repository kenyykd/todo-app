<template>
  <div class="navbar bg-base-100 shadow-sm">
    <div class="navbar-start"></div>
    <div class="tabs tabs-border navbar-center">
      <input
        type="radio"
        name="my_tabs_2"
        class="tab"
        aria-label="首頁"
        checked="checked"
      />
      <input
        type="radio"
        name="my_tabs_2"
        class="tab"
        aria-label="部落格
      "
      />
      <input type="radio" name="my_tabs_2" class="tab" aria-label="留言板" />
    </div>

    <div class="navbar-end">
      <Theme_Controller />
      <SigninModal />
    </div>
  </div>
</template>
<script setup>
import Theme_Controller from "./Theme_Controller.vue";
import SigninModal from "./SigninModal.vue";
</script>

<template>
  <form>

      <!-- NAME -->
    <div class="field-wrapper">
    <label for="name"> Name </label>
    <input id="name" type="text" placeholder="Doe" />
    <popper
      trigger="clickToOpen"
      :options="{
        placement: 'bottom',
        modifiers: {
          offset: { offset: '0,10px' },
        },
      }"
    >
      <div class="popper">Made with vue popper js</div>
      <input type="button" slot="reference" value="infobulle" />
    </popper>
    </div>

    <!-- FIRSTNAME -->
    <div class="field-wrapper">
    <label for="firstname"> Firstname </label>
    <input id="firstname" type="text" placeholder="Jane" />
    <popper
      trigger="clickToOpen"
      :options="{
        placement: 'bottom',
        modifiers: {
          offset: { offset: '0,10px' },
        },
      }"
    >
      <div class="popper">Made with vue popper js</div>
      <input type="button" slot="reference" value="infobulle" />
    </popper>
    </div>
  </form>
</template>

<script>
import Popper from "vue-popperjs";
import "vue-popperjs/dist/vue-popper.css";

export default {
  components: {
    popper: Popper,
  },
};
</script>
<style scoped>
  .field-wrapper {
    margin: 10px;
    padding: 5px;
  }
</style>
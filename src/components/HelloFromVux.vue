<template>
  <div>
    <div class="vux-demo">
      <!-- <img class="logo" src="../assets/vux_logo.png"> -->
      <model-stl :src="modelSrc"></model-stl>
      <h1> </h1>
    </div>
    <group title="cell demo">
      <cell title="VUX" value="cool" is-link></cell>
    </group>
  </div>
</template>

<script>
import { Group, Cell } from 'vux';
import { ModelStl } from 'vue-3d-model';

export default {
  components: {
    Group,
    Cell,
    ModelStl,
  },
  data() {
    return {
      // note: changing this line won't causes changes
      // with hot-reload because the reloaded component
      // preserves its current state and we are modifying
      // its initial state.
      msg: 'Hello World!',
      modelSrc: 'static/右肾脏.stl',
      width: 1500,
      height: 800,
    };
  },
};
</script>

<style>
.vux-demo {
  text-align: center;
}
.logo {
  width: 100px;
  height: 100px;
}
</style>

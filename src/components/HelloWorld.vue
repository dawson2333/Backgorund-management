<script>
import { ref, defineComponent } from "vue";
import { ElButton } from "element-plus";
// defineProps({
//   msg: String,
// });

// const count = ref(0);
export default defineComponent({
  components: {
    ElButton,
  },
  setup() {
    const count = ref(0);
    return {
      count,
    };
  },
});
</script>

<template>
  <h1>{{ msg }}</h1>

  <el-button type="button" @click="count++">count is: {{ count }}</el-button>
</template>

<style scoped>
a {
  color: #42b983;
}
</style>

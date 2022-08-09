<template>
  <div class="app">
  </div>
</template>

<script lang="ts">
import {
  defineComponent, reactive, ref, toRefs,
} from "vue";
import Job from "./types/Job";

export default defineComponent({
  name: "App",
  components: {},
  setup() {
    // const state = reactive({
    //   name: "Link",
    //   age: 25 as number| string,
    // });

    // state.name = "Zelda";
    // state.age = 12;

    // return { ...toRefs(state) };

    // const name = ref("Link");
    // const age = ref<string | number>(13);

    // age.value = 31234;

    // return { name, age };

    const jobs = ref<Job[]>([{
      title: "farm worker", location: "lon lon ranch", salary: 40000, id: "3",
    }]);

    return { jobs };
  },
});
</script>

<style>
</style>

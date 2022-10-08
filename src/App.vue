<template>
  <h2>My Course Goal</h2>
  <!-- Task 1: Output your main course goal with help of the composition API -->
  <!-- Don't hardcode it into the template, instead hardcode it into the JS code -->
  <h3 v-if="toggle">{{ courseGoal }}</h3>
  <!-- Task 2: Toggle (show/ hide) the goal with help of the button  -->
  <button @click="toggleButton">Toggle Goal</button>
  <!-- Task 3: Manage data in three ways -->
  <!-- => Separate refs -->
  <!-- => Ref Object -->
  <!-- => Reactive Object -->
  <!-- Task 4: Also solve the assignment with the Options API -->
</template>

<script>
// import { reactive } from 'vue';

export default {
  // setup() {
  // const courseGoal = ref('Finish the Course!');
  // let toggle = ref(true);
  // const courseData = ref({
  //   goal: 'Finish the Course!',
  //   toggle: true,
  // });

  // const courseData = reactive({
  //   goal: 'Finish the Course!',
  //   toggle: true,
  // });

  // function toggleButton() {
  // toggle.value = !toggle.value;
  // courseData.value.toggle = !courseData.value.toggle;
  // courseData.toggle = !courseData.toggle;
  // }

  // return {courseGoal: courseData.goal, courseData, toggleButton };
  // },

  data() {
    return {
      courseGoal: 'Finish the Course!',
      toggle: true,
    };
  },
  methods: {
    toggleButton() {
      this.toggle = !this.toggle;
    },
  },
};
</script>

<style>
html {
  font-family: sans-serif;
}
body {
  margin: 3rem;
  text-align: center;
}
</style>

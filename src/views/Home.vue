<template>
  <div class="home">
    <tasks />
    <create />
    <notes />
  </div>
</template>

<script>
import create from "../components/tasks/Createtask";
import tasks from "../components/tasks/Tasks";
import notes from "../components/tasks/Notes";
export default {
  name: "Home",
  components: {
    create,
    tasks,
    notes
  }
};
</script>
<style>
.home {
  display: flex;
}
</style>
<template>
  <div class="home">
     <tasks/>
    <create/>
  </div>
</template>

<script>
import create from '../components/tasks/Createtask'
import tasks from '../components/tasks/Tasks'
export default {
  name: 'Home',
  components: {
   create,
   tasks
  },
}
</script>
<style>
.home{
  display: flex;
  
}
</style>
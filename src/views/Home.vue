<template>
  <div class="home">
    <create/>
  </div>
</template>

<script>
import create from '../components/tasks/Createtask'
export default {
  name: 'Home',
  components: {
   create
  },
}
</script>

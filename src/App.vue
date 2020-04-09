<template>
<div>
 <addBlog></addBlog>
</div>
</template>

<script>

import addBlog from './components/addBlog';

export default {
  components:{
    addBlog:addBlog
  },
  data () {
    return {
     
    }
  }
}
</script>

<style>
body{
  margin: 0;
  font-family: 'Nunito SemiBold';
}
</style>

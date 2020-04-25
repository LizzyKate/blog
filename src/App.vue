<template>
<div>
 <!-- <addBlog></addBlog> -->
 <showBlog></showBlog>
</div>
</template>

<script>

import addBlog from './components/addBlog';
import showBlog from './components/showBlog';

export default {
  components:{
    addBlog:addBlog,
    showBlog:showBlog
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

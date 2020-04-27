<template>
<div>
 <!-- <addBlog></addBlog> -->
 <showBlog></showBlog>
 <listBlog></listBlog>
</div>
</template>

<script>

import addBlog from './components/addBlog';
import showBlog from './components/showBlog';
import listBlog from './components/listBlogs';

export default {
  components:{
    addBlog:addBlog,
    showBlog:showBlog,
    listBlog:listBlog
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

<template>
<div v-theme:column="'narrow'" id="show-blog">
    <h1>All Blog Articles</h1>
    <input type="text" v-model="search" placeholder="search blogs">
    <div v-for="(blog, i) in filteredBlogs" :key="i" class="single-blog">
        <h2 v-rainbow>{{blog.title | to-uppercase}}</h2>
    </div>
 
</div>
</template>

<script>

import searchMixin from '../Mixin/searchMixin'

export default {
  
  data () {
    return {
     blogs:[],
     search:''
    }
  },
  methods:{

  },
  created(){
      this.$http.get('http://jsonplaceholder.typicode.com/posts').then(function(data){
          console.log(data);
          this.blogs = data.body.slice(0, 10);
      })
  },
  mixins:[searchMixin]
}
</script>

<style>
#show-blog{
    max-width: 800px;
    margin: 0 auto;
}
.single-blog{
    padding: 20px;
    margin: 20px 0;
    box-sizing: border-box;
    background: #eee;
}
</style>
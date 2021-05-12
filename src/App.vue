<template>
<div class="container">
<div class="row">
<div class="col-md-4">
<Posts @created="refresh"></Posts>
<hr/>
<posts-details v-if="det"></posts-details>
</div></div></div>

  

  

</template>

<script>
import Posts from './components/Posts.vue'
import PostsDetails from './components/PostDetails.vue'
export default {

  name: 'App',
  components: {
    Posts,
    PostsDetails
  },
  data() {
    return {
      selected :'ActiveHobbies',
      model:false,
      det:true,
    }
  },
  methods: {
    showActive(){
      this.selected='ActiveHobbies'
    },
    showInactive(){
      this.selected='InactiveHobbies'
    },
    showModel(){
      this.model=true
    },
    refresh(){
      this.det=false ;
      setTimeout(()=>{
        this.det=true
      },100);


 
    }
  },
}
</script>

<style>
#app {
 
}
</style>

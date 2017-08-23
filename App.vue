<!--Templates-->
<template>
  <div id="app"> 
    <input type="text" v-on:input="changeTitle">
    <p>{{ message }}</p>
</div>
</template>

<!--Javascript-->
<script src="https://unpkg.com/vue/dist/vue.js">
 new Vue({
     el: '#app',
     data:{
         message:'Vue JS is my fav framework' 
     },
     methods:{
         changeTitle: function(){
            this.message = event.target.value;         
         }
     }
 });

</script>

<!--CSS-->

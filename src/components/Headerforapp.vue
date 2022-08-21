<template>

    <header>
        <div v-for="content in contents" :key="content.id">
        <h1 >{{content.text}}</h1>
      
        </div>
      
       
    </header>
</template>
<script lang="ts">
export default{

    data(){
      return{
        contents:[
          {
            id:1,
            text:"Hi My Name is Eby Saju!",
          },
         
        ]
      }
    }
   
    
    
}
</script>
<style scoped>
header{
    display: flex;
    justify-content: space-between;
    align-items: center;
    color: rgb(6, 7, 7);
}
</style>

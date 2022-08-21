<template>
<ul class="menu">
    <div class="menu-indicator"> 
        <li class="menu-item" v-for="link in links" :key="link.id">
         <a href="#" class="menu-link">
            <span>{{link.text}}</span>
         </a>   
        </li>

    </div>

</ul>
  
</template>
<script lang="ts">
export default{

   data()
   {
    return{
        sliderPostion:0,
        selectedElementWidth:0,
        selectedIndex:0,
        links:
        [
            {
             id:1,
            text:"Profile",
            },
            {
             id:2,
            text:"Resume",
            },
             {
             id:2,
            text:"Contact Information",
            }
           
        ]

    }

   }
    
}
</script>
<style >
:root{
    --active-color:#ffee93;
    --link-text-color:#070807;
    --menu-background-color:#12aaf0;
    --active-background-color:#132238;
   
}
.menu {
  padding: 0;
  margin: 0;
  margin-bottom: 35rem;
  position: relative;
  background-color: var(--menu-background-color);
  display: inline-flex;
  border-radius: 4px;
  list-style-type: none;
  overflow: hidden;
  left: 50rem;
  

}

.menu-item {
  display: inline-flex;
}
.menu-link {
  padding: 0.75rem 0.25rem;
  display: inline-flex;
  align-items: center;
  color: var(--link-text-color);
  text-decoration: none;
}
.menu-link:hover,
.menu-link.active {
  color: var(--active-color);
  background-color: var(--active-background-color);
}
</style>
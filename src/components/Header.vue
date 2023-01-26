<template>
    <header>
        <h1>{{ title }}</h1>
        <Button @click="onClick()" text="add task" color="green"/>
    </header>
</template>

<script>
import Button from './Button.vue';

      export default{
             name:'Header',
             props:['title'],
             components:{
                Button
             },
             methods:{
                onClick(){
                    console.log("hi");
                }
             }
      }
</script>
<style scoped>
   header{
    display:flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 20px;
   }
</style>
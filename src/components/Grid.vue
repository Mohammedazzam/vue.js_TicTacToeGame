<template lang="html">
    <div>
      <div class="grid">
         <Cell v-for="n in 9 " :key="n" />
      </div>
    </div>   
</template>

<script>
import  Cell  from "./Cell";
export default{
    name:"Grid",
    components: {
        Cell
    }
}

</script>

<style lang="css" scoped>

.grid{
    display: grid;
    grid-template-columns: 120px 120px 120px ;
    grid-gap: 10px;
    background-color: #34495e;
    color: white;
    width: 100%;
    position: relative;
    padding: 10px;
    box-sizing: border-box;
}



</style>
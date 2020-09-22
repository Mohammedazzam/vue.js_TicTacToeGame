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
    },
    data () {
        return {
            activePlayer:"O",
            gameStatus:"turn",
            gameStatusMessage:"O's Turn",
            gameStatusColor:"statusTurn",
            moves:0,
            winConditions:[
                [1,2,3],[4,5,6],[7,8,9] //row
                [1,4,7],[2,5,8],[3,6,9] //columns
                [1,5,9],[3,5,7] //diagonals
            ],
            cells:{
                1:"",2:"",3:"",
                4:"",5:"",6:"",
                7:"",8:"",9:""
            }
        }
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
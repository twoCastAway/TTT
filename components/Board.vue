<template>
    <div id="board">
        <div class="square" v-for="x in 9" :key="x" @click="setState">
            {{ square[x] }}
        </div>
    </div>
</template>

<style scoped>
#board {
    width: 300px;
    height: 300px;
    margin: 0 auto;
    background-color: grey;
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    justify-content: stretch;
}
h2 {
    text-align: center;
}
.square {
    width: 32.6%;
    border: 1px solid black;
}
</style>

<script>
import { ref } from "vue";

export default {
    name: "board",
    setup() {
        let square = ref([]);
        for(let i = 0; i <= 9; i++) square.value.push(null);

        let currentTurn = "X";
        function setState(){
            currentTurn === "X" ? currentTurn = "O" : currentTurn = "X";
            console.log(currentTurn)
        }

        return { square, currentTurn, setState }
    }
}
</script>
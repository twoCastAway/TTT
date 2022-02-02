<script>
export default {
    data() {
        return {
            squares: [
                [0,1,2],
                [3,4,5],
                [6,7,8]
            ]
        }
    },
}
</script>

<template>
    <div class="board" v-for="(col, colID) in squares" :key="colID">
        <div class="square" v-for="(row, rowID) in squares" :key="rowID">
            {{ col[rowID] }}
        </div>
    </div>
</template>

<style>
.board {
    display: flex;
}
.square {
    width: 64px;
    height: 64px;
    border: 2px solid black;
    text-align: center;
}
</style>
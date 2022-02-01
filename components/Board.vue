<script>
export default {
    data() {
        return {
            squares: {
                row1:[0,1,2],
                row2:[3,4,5],
                row3:[6,7,8]
            }
        }
    }
}
</script>

<template>
    <!-- <div id="board" v-for="row in 3" :key="row">
        <div id="board" v-for="(row, index) in 3" :key="index">
            <div :id="`row${index}`" class="row" v-for="(square, index) in 3" :key="index">
                <div :id="`square${index}`" class="square">
                    {{ index }}
                </div>
            </div>
        </div>         
        <Row />
    </div> -->



    <div v-for="(value, index) in squares[0]" :key="index">
        <!-- <div v-for="(value, row) in squares" :key="row">
            <div :v-for="(value, square) in `row${row}`" :key="square">
                {{ value }}
            </div>
        </div> -->
        {{ value }}
    </div>
</template>

<style>
#board {
    display: flex;
}
#square {
    width: 64px;
    height: 64px;
    border: 2px solid black;
}
</style>
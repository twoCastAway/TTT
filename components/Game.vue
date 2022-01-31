<script lang="ts">
const board_states = {
                empty: 0b000000000,
                fill: 0b111111111,
                wins: [
                    0b111000000,
                    0b000111000,
                    0b000000111,
                    0b100100100,
                    0b010010010,
                    0b001001001,
                    0b100010001,
                    0b001010100
                ],
            };

console.log(~board_states.wins[2]);
</script>

<template>
    <div id="wrapper">
        <h1>TicTacToe</h1>
        <div id="game">
            <Board />
        </div>
        <button onclick="reset_board">game start</button> 
    </div>
</template>

<style>
#wrapper {
    width: 300px;
    height: 300px;
    position: relative;
    margin: 0 auto;
}
#game {
    position: absolute;
    top: 15%;
    left: 15%;
    margin-top: 10px;
}
h1 {
    text-align: center;
}
button {
    position: absolute;
    top: 90%;
    left: 36%;
    margin: 0 auto;
    border-radius: 10px;
}
</style>
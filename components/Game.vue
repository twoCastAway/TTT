<script lang="ts">

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
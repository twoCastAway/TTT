<template>
    <div id="app">
        <Game />
    </div>
</template>

<style>
#app {
    width: max-content;
    margin: 0 auto;
}
.game {
    width: 300px;
    height: 300px;
    margin: 0;
}
h1 {
    text-align: center;
}
.row {
    margin: 0 auto;
    display: flex;
    justify-content: center;
}
.square {
    width: 64px;
    height: 64px;
    border: 2px solid black;
    text-align: center;
}
</style>
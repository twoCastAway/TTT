<template>
    <div id="board" v-for="row in 3" :key="row">
        <Row />
    </div>
</template>

<style>
#board {
    display: flex;
}
</style>
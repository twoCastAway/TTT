<script lang="ts">

</script>

<template>
    <div v-for="square in 3" :key="square">
        <div id="square">
            
        </div>
    </div>
</template>

<style>
#square {
    width: 64px;
    height: 64px;
    border: 2px solid black;
}
</style>
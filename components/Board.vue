<template>
    <div class="row" v-for="x in 3" :key="x">
        <button class="square" v-for="y in 3" :key="y" @click="move">
            {{ squares[x][y] }}
        </button>
    </div>
</template>

<script>
import { ref } from "vue"

export default {
    setup() {
        let squares = ref([
            ['','',''],
            ['','',''],
            ['','','']
        ])
        const move = () => {
            squares.value = 'O'
        }

        return { squares, move }
    }
}
</script>
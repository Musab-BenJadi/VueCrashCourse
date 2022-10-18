<template>
    <header>
        <h1>{{title}}</h1>
        <Button text="Add Task" color="green" />
    </header>
</template>

<script>

import Button from './Button'
import { stringLiteral } from '@babel/types';

    export default {
        name: 'Header',
        props: {
            title: String,
        // other metod to bring data with default string
        //     title: {
        //         type: String,
        //         default: 'header section',
        // },
    },
    components: {
        Button
    }
}
</script>

<style scoped>
    header {
        display: flex;
        justify-content: space-between;
        align-items: center;
        margin-bottom: 20px;
    }
</style>
<template>
    <tbody>
        <tr v-for="(item, i) in bodyContent" v-bind:key="i">
            <td>{{item}}</td>
        </tr>
    </tbody>

</template>


<script>
    export default {
        name: "TableBody",
        props: ['bodyContent'],
    }
</script>


<style scoped>

</style>


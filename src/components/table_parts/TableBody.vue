<template>
    <tbody>
        <tr v-for="(item, i) in bodyContent" v-bind:key="i">

            <td v-for="(data, key) in headerContent" v-bind:key="key">
              {{item[key]}}
            </td>
        </tr>
    </tbody>

</template>


<script>
    export default {
        name: "TableBody",
        props: ['headerContent', 'bodyContent']
    }
</script>


<style scoped>

</style>


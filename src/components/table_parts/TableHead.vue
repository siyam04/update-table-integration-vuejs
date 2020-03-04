<template>

    <thead>
        <tr>
            <th v-for="(item, i) in headerContent" v-bind:key="i" scope="col" @click="sorting(item)">
                <a href="#">{{item}}</a>
            </th>
        </tr>
    </thead>

</template>


<script>
    export default {
        name: "TableBody",
        props: ['headerContent'],

        methods: {
            sorting(param){
                console.log(param)

            }
        }
    }
</script>


<style scoped>

</style>


<template>

    <div class="container">

        <h1>Users</h1>
        <br><br>

        <table class="table">
            <TableHead v-bind:headerContent="headerContent"></TableHead>
            <TableBody v-bind:bodyContent="bodyContent"></TableBody>
        </table>

        <button class="btn btn-dark">
            <router-link :to="{name: 'Players'}">GoTo Players</router-link>
        </button>
    </div>

</template>


<script>

    import TableHead from "../table_parts/TableHead";
    import TableBody from "../table_parts/TableBody";


    export default {
        name: "User",
        components: {TableHead, TableBody},
        data() {
            return {
                headerContent: {
                    serial: 'SERIAL',
                    name: 'NAME',
                    age: 'AGE',
                },
                bodyContent: [
                    {
                        serial: 'data',
                        name: 'data',
                        age: 'data',
                    },
                    {
                        serial: 'data',
                        name: 'data',
                        age: 'data',
                    },
                    {
                        serial: 'data',
                        name: 'data',
                        age: 'data',
                    },
                ]

            }
        },
    }
</script>


<style scoped>

</style>
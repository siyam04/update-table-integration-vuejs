<template>

    <div class="container">
        <h1>Players</h1>
        <br><br>

        <table class="table">
            <TableHead v-bind:headerContent="headerContent"></TableHead>
            <TableBody v-bind:bodyContent="bodyContent">></TableBody>
        </table>

        <button class="btn btn-dark">
            <router-link :to="{name: 'User'}">GoTo User</router-link>
        </button>

    </div>

</template>


<script>
    import TableHead from "../table_parts/TableHead";
    import TableBody from "../table_parts/TableBody";


    export default {
        name: "Players",
        components: {TableHead, TableBody},
        data() {
            return {
                headerContent: {
                    serial: 'SERIAL',
                    player_name: 'PLAYER NAME',
                    score: 'SCORE',
                },
                bodyContent: [
                    {
                        player_name: 'data',
                        serial: 'data',
                        score: 'data',
                    },
                    {
                        serial: 'data',
                        player_name: 'data',
                        score: 'data',
                    },
                    {
                        score: 'data',
                        serial: 'data',
                        player_name: 'data',
                    },
                ]
            }
        }
    }
</script>


<style scoped>


</style>


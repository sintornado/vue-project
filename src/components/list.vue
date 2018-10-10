<template>
    <div class="container">
                <table class="table table-hover table-primary container">
                    <tbody>
                        <tr @click="$emit('current-user-change', client)" class="row-box">
                            <th><img v-bind:src='photo' alt="photo" class="image-size"></th>
                            <td>{{ first }}</td>
                            <td>{{ last }}</td>
                            <td><button variant="danger" @click="$emit('delete-worker', client)">Danger</button></td>
                        </tr>
                    </tbody>
                </table>
            </div>
</template> 
<script>
    export default {
        props: ['first', 'last', 'photo', 'client'],
        methods: {
        }
    }
</script>
<style>
    .image-size {
        width: 50px;
        height: 50px;
        border-radius: 20px;
    }

    .row-box {
        box-shadow: 0 0 10px rgba(0,0,0,0.5);
        
    }
</style>
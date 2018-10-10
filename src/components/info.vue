<template>
        <div class="jumbotron jumbotron-fluid container">
            <div class="container">
                <h1 class="display-4">Information about worker:</h1>
                <hr>
                <img v-bind:src='client.general.avatar' alt="photo"></th>
                <br>
                <p>{{client.general.firstName}} {{client.general.lastName}}</p>
                <br>
                <h3>Job:</h3>
                <p>Company: {{client.job.company}} {{client.job.title}}</p>
                <p>Title: {{client.job.title}}</p>
                <br>
                <h3>Contact:</h3>
                <p>Email: {{client.contact.email}} {{client.contact.phone}}</p>
                <p>Phone: {{client.contact.phone}}</p>
                <br>
                <h3>Adress:</h3>
                <p> Street: {{client.address.street}} </p>
                <p> City: {{client.address.city}}</p>
                <p> Zip-code: {{client.address.zipCode}}</p>
                <p> Country: {{client.address.country}}</p>
            </div>
        </div> 
</template>
<script>
    export default {
        props:['client'],
    }
</script>
<style>
    
</style>
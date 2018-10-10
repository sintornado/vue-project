<template>
    <div class="container">
        <div> <h3>Search:</h3></div>
        <div class="input-group mb-3">
            <input type="text" v-model='search' @keyup="$emit('input-search', search)" class="form-control" placeholder="" aria-label="Example text with button addon" aria-describedby="button-addon1">
        </div>
        <button v-on:click='clickOk'>ok</button>
        <p>{{search}}</p>
    </div>
</template>
<script>
    export default { 
        data(){
            return{
                search: ''
            }
        },
        computed: {
        },
        methods: {
            clickOk(){
                console.log(this.search);
            }
        }
    }
</script>
<style>
    
</style>
<template>

    <div class="my-card m-2">
        <div class="block-title">
            <h1> <router-link id="link" :to="{path: '/oneNew/'+ info.id}">{{info.title}}</router-link></h1>
        </div>
        
        <div class="block-text p-2">
            <p>index {{info.id}}</p>
            <p>{{info.by}}</p>
            <p>{{info.ff}}</p>
        </div>
    </div>

</template>

<script>
    export default {
        name: 'cardX',
        props:['info']
    }
</script>

<style scoped>
    .my-card {
        min-height: 150px;
        min-width: 400px;
        background-color: #141634;
        border-radius: 20px;
        box-shadow: rgba(0, 0, 0, 0.24) 0px 3px 8px;
    }
    .block-text{
        background-color: rgb(167, 181, 219);
        height: auto;
        border-bottom-left-radius: 20px;
        border-bottom-right-radius: 20px;
    }
    .block-title{
        display: flex;
        flex-direction: row;
        justify-content: center;
    }
    .block-title #link{
        color: white;
        text-decoration: none;
        
    }
    .block-title #link:hover{
        color: rgb(0, 68, 255);
        text-decoration: none;
        
    }
</style>
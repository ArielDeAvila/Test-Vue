<script setup>

</script>

<template>
    <form >
        <input type="text" placeholder="   Search here">
        <button type="button"><img src="/search.png" alt="search" ></button>
    </form>
    
</template>

<style scoped>
    form{
        background-color: #1C2126;
        border-radius: 0.63vw;
        border: 1px solid #2F363D;
        padding-right: 1.25vw;

        display: flex;
        justify-content: space-between;
        align-items: center;

        width: 39.17vw;
        height: 2.92vw;
    

    }


    input[type="text"] {
        all: unset;
        width: 80%;
        height: 2.92vw;
        caret-color: var(--background-green);
        
        text-align: left;
        padding: 0 15px;

        font-size: 0.83vw;

    }
    
    button{
        padding: 0;
        height: 35px;
        border-radius: 15px;
        background-color: transparent;
        border-color: transparent;

       
    }

    button img{
        width: 1.25vw;
        height: 1.25vw;
        
    }

    button:hover{
        border-color: transparent;
        cursor: pointer;

    }

    button:focus{
        outline: 0;
    }

    

</style>

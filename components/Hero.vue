<template>
    <div class="Hero container">
        <div class="text-container">
            <h1 class="header">Find your Fire Extinguisher</h1>
            <p class="snippet">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Iste iusto illum quidem asperiores, cum nisi aperiam eius ipsa sapiente odit!</p>
            <a href="/products"><button class="button btn">Start Looking</button></a>
            
            
        </div>
        <img src="~assets/svg/fire-extinguisher.svg" alt="fire-extinguisher" class="image">
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style scoped>
    .Hero {
        display: flex;
    }

    .header {
        font-size: 2rem;
    }
    
    .snippet {
        color: grey;
        font-size: 1.25rem;
    }
    .image {
        width: 12.5rem;
        margin-top: 1rem;
    }
    .overlay {
        background: rgba(0, 0, 0, 0);
        position: absolute;
        width: 100%;
        height: 100%;
        top: 0;
    }
    .button {
        padding: 1rem 4rem;
        border-radius: 75rem;
        background-color: rgb(231, 81, 43);
        color: white;
        width: 20rem;
        font-weight: 700;
        transition: 0.5s;
        margin-top: 50px;
    }
    .button:hover {
        width: 21.5rem;
    }
    @media (max-width: 500px) {
        .Hero {
            height: 40vh;
        }
    }
</style>
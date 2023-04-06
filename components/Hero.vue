<template>
    <div class="Hero container">
        <div class="text-container">
            <h1 class="header">Find your Fire Extinguisher</h1>
            <p class="snippet"> Lorem ipsum dolor sit amet consectetur, adipisicing elit. Et quia rem iure. Recusandae dolorem rem quis a dolore. Et, voluptas!</p>
            <button class="button btn">Start Looking</button>
        </div>
        <img class="image" src="~assets/fire-extinguisher.svg" alt="fire extinguisher">
    </div>
</template>

<script> 

export default {

}
</script>

<style scoped>
.Hero {
    height: 60vh;
    position: relative;
    display: flex;
    padding: 5rem 0;
    align-items: flex-start;
    justify-content: space-between;
}

.text-container {
    width: 50%;
    margin-top: 3rem;
}

.header {
    font-weight: 950;
    font-size: 4.5rem;
}

.snippet {
    color: grey;
    font-size: 1.25rem;
    font-weight: bold;
}

.image {
    width: 27rem;
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
    padding: 12px 4rem;
    border-radius: 100rem;
    background-color: rgb(231, 81, 43);
    color: white;
    width: 20rem;
    font-weight: 700;
    transition: 0.5s;
}

.button:hover {
    width: 21.5rem;
}

@media (max-width: 500px) {
    .Hero {
        height: 40vh;
    }
}</style>
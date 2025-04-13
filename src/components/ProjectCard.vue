<script setup>
defineProps({
    title: String,
    description: String,
    image: String,
    link: String
})
</script>

<template>
    <div class="project-card">
        <img :src="image" class="project-image" alt="">
        <p>{{ title }}</p>
        <h3>{{ description }}</h3>
        <a :href="link" target="_blank" class="button">See more</a>
    </div>
</template>

<style scoped>
.project-card {
    font-size: 1.5rem;
    font-weight: 15rem;
    border: 5px solid black;
    border-radius: 15px;
    padding: 2rem 1.5rem;
    width: 30rem;
    text-align: center;
    margin-top: 8rem;
    background-color: #F2EFE7
}

.project-card p{
    font-weight: 500;
    color: #006A71;
}

.project-image {
    width: 100%;
    max-width: 200px;
    border-radius: 8px;
    object-fit: cover;
    margin-bottom: 1rem;
    aspect-ratio: 16/16;
}

.button {
    display: inline-block;
    margin-top: 12px;
    padding: 0.8rem 2rem;
    background-color: #f0eada;
    border-radius: 4rem;
    font-size: 1.5rem;
    font-weight: 600;
    color: black;
    text-decoration: none;
    border: 2px solid black;
    transition: 0.3s ease;
    cursor: pointer;
}

.button:hover {
    transform: scale(1.05);
    background-color: #006A71;
    color: white;
    box-shadow: 0 0 15px #006A71;
}
</style>

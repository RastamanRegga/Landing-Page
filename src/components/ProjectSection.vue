<script setup>
import ProjectCard from './ProjectCard.vue';

const projects = [
    {
        title: 'To-Do List App',
        description: 'Simple App using java and python',
        image: require('@/src/assets/todo.png'),
        link: 'https://github.com/RastamanRegga/To-Do-App'
    },
    {
        title: 'Landing Page',
        description: 'Responsive landing page using Vue.js',
        image: require('@/src/assets/web.png'),
        link: '#home'
    },
    {
        title: 'Restful API',
        description: 'Built Restful API for login with react.js',
        image: require('@/src/assets/api.png'),
        link: 'https://github.com/RastamanRegga/RESTFUL-API'
    },
    {
        title: 'Calculator App',
        description: 'Making Android Calculator with kotlin',
        image: require('@/src/assets/kalkulator.jpg'),
        link: 'https://github.com/RastamanRegga/Kalkulator'
    }
]
</script>

<template>
    <section id="Project">
        <h1>My Project</h1>
        <div class="project-list">
            <ProjectCard v-for="(project, index) in projects" :key="index" :title="project.title"
                :description="project.description" :image="project.image" :link="project.link" />
        </div>
    </section>
</template>

<style scoped>
.project-list {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 4rem;
    padding: 2rem;
}

section {
    background-color: #f0eada;
}

section h1 {
    text-align: center;
    font-size: 4rem;
    color: #006A71;
}
</style>
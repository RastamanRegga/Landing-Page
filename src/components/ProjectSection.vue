<script setup>
import ProjectCard from './ProjectCard.vue'
import todoImg from '../assets/todo.png'
import webImg from '../assets/web.png'
import apiImg from '../assets/api.png'
import kalkulatorImg from '../assets/kalkulator.png'

const projects = [
    {
        title: 'To-Do List App',
        description: 'Simple App using java and python',
        image: todoImg,
        link: 'https://github.com/RastamanRegga/To-Do-App'
    },
    {
        title: 'Landing Page',
        description: 'Responsive landing page using Vue.js',
        image: webImg,
        link: '#home'
    },
    {
        title: 'Restful API',
        description: 'Built Restful API for login with react.js',
        image: apiImg,
        link: 'https://github.com/RastamanRegga/RESTFUL-API'
    },
    {
        title: 'Calculator App',
        description: 'Making Android Calculator with kotlin',
        image: kalkulatorImg,
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
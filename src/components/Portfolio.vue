<template>
    <div class="portfolio">
        <div v-bind:key="project" v-for="project in projects" class="project">
            <h2 class="project__title">{{ project.title }}</h2>
            <p class="project__desc">{{ project.description }}</p>
            <a :href="project.url" class="project__link">{{ project.url }}</a>
        </div>
    </div>
</template>

<script>
export default {
    props: ['projects']
}
</script>

<style lang="scss">
    .portfolio {
        display: grid;
        
        grid-gap: 30px;

        @media (min-width: 768px){
            grid-template-columns: repeat(2, 1fr);
        }
    }
</style>
<template>
    <div class="portfolio">
        <div v-bind:key="project" v-for="project in projects">
            was
        </div>
    </div>
</template>

<script>
export default {
    props: ['projects']
}
</script>
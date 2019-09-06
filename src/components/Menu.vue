<template>
    <ul class="menu menu--horizontal">
        <li><a href="#competences">Compétences</a></li>
        <li><a href="#parcours">Parcours</a></li>
        <li><a href="#realisations">Réalisations</a></li>
        <li><a href="#contact">Contact</a></li>
    </ul>
</template>

<style lang="scss" scoped>
    .menu {
        margin: 0;
        padding: 0;
        list-style: none;

        &--horizontal {
            display: flex;

            li:not(:last-child){
                margin-right: 1rem;
            }
        }
    }
</style>
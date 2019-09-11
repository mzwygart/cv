<template>
    <ul class="checklist">
        <li v-bind:key="item" v-for="item in items"><CheckIcon class="icon" />{{ item }}</li>
    </ul>
</template>

<script>
import CheckIcon from '~/assets/icons/Check.svg'

export default {
    props: ['items'],
    components: {
        CheckIcon
    }
}
</script>

<style lang="scss" scoped>
.checklist {
    list-style: none;

    li {
        margin: 0
    }

    svg {
        fill: $contrast;
        margin-right: .5em;
        transform: translateY(.2em)
    }
}
</style>

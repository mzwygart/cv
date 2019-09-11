<template>
    <div class="timelineItem__wrapper clearfix">
        <div v-bind:key="entry" v-for="entry in entries" class="timelineItem">
            <h2 class="timelineItem__title">{{ entry.title }}</h2>
            <time class="timelineItem__date">{{ entry.year }}</time>
            <p>{{ entry.description }}</p>
        </div>
    </div>
</template>

<script>
    export default {
        props: ['entries']
    }
</script>

<style lang="scss">
    .timelineItem {
        margin: 1rem 0 1rem 3rem;
        padding: 2rem 3rem;
        border: 1px solid #333;
        position: relative;
        overflow: visible;

        &::before {
            display: inline-block;
            content: '●';
            position: absolute;
            top: 0; left: -10px;
            transform: translateX(-50%);
            color: $contrast;
            font-size: 2rem;
        }

        @media (min-width: 768px){
            width: calc(50% - 3rem);
            margin: 1rem 3rem 1rem 0;

            &:nth-child(even) {
                margin: 1rem 0 1rem 3rem;
                margin-left: auto;
            }
        }

        &__wrapper {
            position: relative;

            &::before {
                content: '';
                display: block;
                position: absolute;
                width: 5px;
                top: 1rem; bottom: 1rem; left: 0;
                transform: translateX(-50%);
                background: $contrast;
            }

            @media (min-width: 768px){
                &::before {
                    left: 50%;
                }
            }
        }

        &__title {
            font-size: 1.8rem;
            display: inline-block;
            margin-right: 1rem;
        }

        &__date {
            font-size: 1.6rem;
            display: inline-block;

            &::before {
                display: inline-block;
                content: '●';
                font-size: .5rem;
                vertical-align: middle;
                margin-right: 1rem;
            }
        }
    }
</style>
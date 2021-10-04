<template>
    <li :class="['card', cardType]">
        <h4>{{ header }}</h4>
        <p>{{ info }}</p>
    </li>
</template>

<script>
export default {
    props: {
        header: { type: String, required: true },
        info: { type: String, required: true },
        cardType: { type: String, default: '' },
    },
};
</script>

<style scoped>
.card {
    list-style: none;
    line-height: 1.7rem;
}

.card h4 {
    color: var(--box);
    font-size: 1.3rem;
    text-transform: uppercase;
}

.card p {
    color: var(--text-light-gray);
}

.card.info h4 {
    font-size: 0.8rem;
    color: var(--text-light-gray);
}

.card.info p {
    font-size: 1.1rem;
    color: var(--dark-gray);
}
</style>

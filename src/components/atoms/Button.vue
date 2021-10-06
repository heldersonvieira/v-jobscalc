<template>
    <button @click="goTo(route)" :class="['primary', color]">
        <img v-if="img" src="@/assets/img/plus.svg" alt="Adicionar novo Job" />
        {{ title }}
    </button>
</template>

<script>
export default {
    props: {
        route: { type: String, required: true },
        title: { type: String, required: true },
        color: { type: String },
        img: { type: Boolean, default: false },
    },

    methods: {
        goTo(route) {
            this.$router.push({ name: route });
        },
    },
};
</script>

<style scoped>
.primary {
    display: flex;
    align-items: center;
    gap: 2rem;
    font-family: IBM Plex Sans;
    font-size: 1rem;
    font-weight: bold;
    letter-spacing: 0.1rem;
    text-transform: uppercase;
    border: none;
    border-radius: 5px;
    background: var(--green);
    color: var(--box);
    cursor: pointer;
    transition: all 0.2s ease;
}

.primary:hover {
    opacity: 0.8;
}

.primary img {
    background: var(--orange-hover);
    padding: 0.2rem;
    margin-left: 0.5rem;
    border-radius: 5px;
}

.red {
    background: var(--red);
}

.orange {
    background: var(--orange);
}

.gray {
    background: var(--text-light-gray);
    color: var(--text-gray);
}
</style>

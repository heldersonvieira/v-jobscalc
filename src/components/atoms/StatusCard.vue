<template>
    <div :class="['status-card', done ? 'done' : '']">
        <p>{{ done ? (text = 'Encerrado') : text }}</p>
    </div>
</template>

<script>
export default {
    data() {
        return {
            text: 'Em andamento',
        };
    },

    props: {
        done: { type: Boolean, default: false },
    },
};
</script>

<style scoped>
.status-card {
    padding: 0.8rem 2rem;
    border-radius: 5rem;
    background: var(--low-green);
    color: var(--green);
    text-align: center;
}

.done {
    background: var(--low-red);
    color: var(--red);
}
</style>

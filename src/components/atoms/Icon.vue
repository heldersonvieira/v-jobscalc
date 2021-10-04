<template>
    <img
        class="icon"
        :src="require(`@/assets/img/${name}.svg`)"
        alt="Editar job"
    />
</template>

<script>
export default {
    props: { name: { type: String, required: true } },
};
</script>

<style scoped>
.icon {
    border-radius: 5px;
    border: 1px solid var(--text-light-gray);
    padding: 0.5rem;
    cursor: pointer;
    transition: all 0.3s ease;
}

.icon:hover {
    background: var(--background);
}
</style>

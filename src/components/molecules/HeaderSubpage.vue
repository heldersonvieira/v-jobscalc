<template>
    <header class="header-subpage">
        <div class="container">
            <img
                @click="goBack()"
                src="@/assets/img/arrow.svg"
                alt="Seta para voltar"
            />
            <h2>{{ subtitle }}</h2>
        </div>
    </header>
</template>

<script>
export default {
    props: {
        subtitle: { type: String, required: true },
        route: { type: String, required: true },
    },

    methods: {
        goBack() {
            this.$router.push({ name: this.route });
        },
    },
};
</script>

<style scoped>
.header-subpage {
    background: var(--dark-purple);
    height: 120px;
}

.container {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    height: 100%;
    align-items: center;
}

.container h2 {
    grid-column-start: 2;
    margin: 0 auto;
    font-size: 1.2rem;
    color: var(--text-light-gray);
}

img {
    cursor: pointer;
}
</style>

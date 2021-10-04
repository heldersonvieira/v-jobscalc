<template>
    <div class="free__hours">
        <img src="@/assets/img/alert.svg" alt="Alerta de horas livres" />
        <h2>Você tem 2 horas livre no seu dia</h2>
    </div>
</template>

<script>
export default {};
</script>

<style scoped>
.free__hours {
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 0.8rem;
    width: 400px;
    font-size: 0.8rem;
    color: var(--box);
}

.free__hours img {
    width: 25px;
}
</style>

<template>
    <section class="profile-card">
        <div class="profile">
            <Avatar />
            <h3>Jaqueline</h3>
        </div>
        <div class="hourly-value">
            <p>O valor da sua hora é <strong>R$ 75,00 reais</strong></p>
        </div>
        <Button route="Home" title="Salvar Dados" />
    </section>
</template>

<script>
import { Avatar, Button } from '@/components';

export default {
    components: { Avatar, Button },
};
</script>

<style scoped>
.profile-card {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-between;
    color: var(--text-gray);
    background: var(--box);
    width: 45%;
    height: 80%;
    padding: 4rem;
}

.profile {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 1.2rem;
    width: 100%;
    font-size: 1.6rem;
}

.avatar {
    width: 90%;
}

.hourly-value {
    width: 100%;
    font-size: 1.5rem;
    text-align: center;
}

.primary {
    display: flex;
    justify-content: center;
    width: 100%;
    height: 60px;
    font-size: 0.9rem;
}
</style>

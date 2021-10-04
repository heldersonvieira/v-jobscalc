<template>
    <Container>
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
    </Container>
</template>

<script>
import { Container, Avatar, Button } from '@/components';

export default {
    components: { Container, Avatar, Button },
};
</script>

<style scoped>
.container {
    display: flex;
    align-items: center;
    height: calc(100vh - 120px);
}
.profile-card {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-between;
    color: var(--text-gray);
    background: var(--box);
    width: 32%;
    height: 78%;
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

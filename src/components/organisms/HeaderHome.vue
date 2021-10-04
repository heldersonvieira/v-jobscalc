<template>
    <header class="header">
        <div class="container">
            <div class="principal">
                <Logo />
                <AvailableTime />
                <ProfileHome />
            </div>
            <div class="panel">
                <div class="cards">
                    <Card header="12" info="Projetos ao total" />
                    <Card header="7" info="Em andamento" />
                    <Card header="4" info="Encerrados" />
                </div>
                <Button
                    route="Job"
                    title="Adicionar Novo Job"
                    color="orange"
                    :img="true"
                />
            </div>
        </div>
    </header>
</template>

<script>
import { Logo, ProfileHome, AvailableTime, Button, Card } from '@/components';

export default {
    components: { Logo, ProfileHome, AvailableTime, Button, Card },
};
</script>

<style scoped>
.header {
    height: 32vh;
    background: var(--dark-purple);
}

.principal {
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 120px;
    border-bottom: 1px solid var(--text-dark-gray);
}

.panel {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding-top: 2rem;
}

.cards {
    display: flex;
    justify-content: flex-start;
    gap: 2rem;
    padding: 0;
}

.primary {
    width: 300px;
    height: 60px;
    font-size: 0.9rem;
}
</style>

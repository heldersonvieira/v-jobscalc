<template>
    <li class="about-job">
        <div class="name">
            <p class="id">1</p>
            <p>Pizzaria Guloso</p>
        </div>
        <ul class="cards">
            <Card header="Prazo" info="3 dias para entrega" cardType="info" />
            <Card header="Valor" info="R$ 4500,00" cardType="info" />
        </ul>
        <StatusCard />
        <div class="icons-group">
            <Icon name="trash" />
            <Icon name="edit-3" />
        </div>
    </li>
</template>

<script>
import { Card, StatusCard, Icon } from '@/components';

export default {
    components: { Card, StatusCard, Icon },
};
</script>

<style scoped>
.about-job {
    display: grid;
    grid-template-columns: 2fr 2fr 1fr 1fr;
    align-items: center;
    justify-content: flex-start;
    background: var(--box);
    height: 110px;
    border-radius: 5px;
    border-left: 4px solid var(--box);
    padding: 0 2rem;
    margin-bottom: 0.8rem;
}

.about-job:hover {
    background: linear-gradient(90deg, #ffe5ca 0.45%, #fafafa 34%);
    border-left: 4px solid var(--orange);
}

.name {
    display: flex;
    align-items: center;
    gap: 2rem;
}

.name .id {
    color: var(--text-light-gray);
    font-size: 1.2rem;
}

.name p {
    font-family: IBM Plex Sans;
    font-size: 1.6rem;
    font-weight: bold;
    letter-spacing: 0.05rem;
    color: var(--text-gray);
}

.cards {
    display: flex;
    justify-content: flex-start;
    gap: 4rem;
    padding: 0;
}

.icons-group {
    justify-self: flex-end;
    display: flex;
    align-items: center;
    gap: 0.6rem;
    width: 50%;
    height: 50%;
}
</style>

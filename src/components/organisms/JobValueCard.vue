<template>
    <div class="job-value-card">
        <img src="@/assets/img/no-cash.svg" alt="Image de dinheiro" />
        <p>{{ messages[0] }}</p>
        <div class="buttons-group">
            <Button route="Home" title="Salvar" />
            <Icon name="trash" />
        </div>
    </div>
</template>

<script>
import { Button, Icon } from '@/components';

export default {
    components: { Button, Icon },

    data() {
        return {
            messages: [
                'Preencha os dados ao lado para ver o valor do projeto',
                'O valor do projeto ficou em ',
            ],
        };
    },
};
</script>

<style scoped>
.job-value-card {
    background: var(--box);
    color: var(--text-gray);
    width: 32%;
    height: 365px;
    padding: 3rem;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    align-items: center;
}

.job-value-card > img {
    width: 40%;
}

.buttons-group {
    width: 100%;
    display: flex;
    justify-content: space-between;
}

.buttons-group .primary {
    width: 77%;
    height: 50px;
    display: flex;
    justify-content: center;
}

.buttons-group img {
    padding: 0 0.7rem;
}
</style>

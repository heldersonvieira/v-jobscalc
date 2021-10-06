<template>
    <div class="job">
        <HeaderSubpage subtitle="Adicionar novo Job" />
        <Container>
            <form>
                <h3>Dados do Job</h3>
                <fieldset>
                    <Input class="name-input" label="Nome do Job" />
                    <Input
                        class="standart-input"
                        label="Quantas horas por dia vai dedicar ao Job?"
                    />
                    <Input
                        class="standart-input"
                        label="Estimativa de horas para esse job?"
                    />
                </fieldset>
            </form>
            <JobValueCard />
        </Container>
    </div>
</template>

<script>
import { HeaderSubpage, Container, JobValueCard, Input } from '@/components';

export default {
    components: { HeaderSubpage, Container, JobValueCard, Input },
};
</script>

<style scoped>
.container {
    display: flex;
    padding-top: 6rem;
    gap: 6rem;
    height: calc(100vh - 120px);
}

form {
    width: 57%;
    height: 400px;
}

form h3 {
    border-bottom: 1px solid var(--text-light-gray);
    padding-bottom: 0.6em;
    margin-bottom: 2rem;
    font-size: 2rem;
    color: var(--text-gray);
}

fieldset {
    border: none;
    padding: 0;
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;
}

.name-input {
    width: 100%;
    margin-bottom: 3rem;
}

.standart-input {
    width: 48%;
}
</style>

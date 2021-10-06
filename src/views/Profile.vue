<template>
    <div class="profile">
        <HeaderSubpage subtitle="Meu perfil" />
        <Container>
            <ProfileCard />
            <form>
                <fieldset>
                    <h4>Dados do perfil</h4>
                    <div class="input-group">
                        <Input placeholder="Nome" />
                        <Input placeholder="Link da foto" />
                    </div>
                </fieldset>
                <fieldset>
                    <h4>Planejamento</h4>
                    <div class="input-group">
                        <Input
                            label="Quanto eu quero ganhar por mês?"
                            placeholder="R$"
                        />
                        <Input label="Quantas horas quero trabalhar por dia?" />
                        <Input
                            label="Quantos dias quero trabalhar por semana?"
                        />
                        <Input
                            label="Quantas semandas por ano você quer tirar férias?"
                        />
                    </div>
                </fieldset>
            </form>
        </Container>
    </div>
</template>

<script>
import { HeaderSubpage, ProfileCard, Container, Input } from '@/components';

export default {
    components: { HeaderSubpage, ProfileCard, Container, Input },
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
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    width: 100%;
    height: 80%;
}

fieldset {
    border: none;
}

.input-group {
    display: flex;
    flex-wrap: wrap;
    gap: 2rem;
}

fieldset h4 {
    border-bottom: 1px solid var(--text-light-gray);
    padding-bottom: 0.6em;
    margin-bottom: 2rem;
    font-size: 2rem;
    color: var(--text-gray);
}

.input-box {
    width: 47.5%;
}
</style>

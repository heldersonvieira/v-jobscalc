<template>
    <div class="modal-overlay hidden">
        <div class="modal">
            <img src="@/assets/img/trash.svg" alt="Icone lixeira" />
            <h2>Excluir Job</h2>
            <p>Quer mesmo excluir esse job?</p>
            <div class="buttons-group">
                <Button route="Home" title="Cancelar" color="gray" />
                <Button route="Home" title="Excluir Job" color="red" />
            </div>
        </div>
    </div>
</template>

<script>
import { Button } from '@/components';

export default {
    components: { Button },
};
</script>

<style scoped>
.modal-overlay {
    width: 100%;
    height: 100%;
    background: rgba(0, 0, 0, 0.7);
    position: fixed;
    top: 0;
    display: flex;
    align-items: center;
    justify-content: center;
    z-index: 999;
}
.modal {
    background: var(--box);
    color: var(--text-gray);
    font-size: 1.2rem;
    width: 448px;
    height: 340px;
    border-radius: 5px;
    padding: 3rem;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    align-items: center;
}

.modal > img {
    width: 15%;
}

.modal h2 {
    font-size: 2rem;
}

.buttons-group {
    width: 100%;
    display: flex;
    justify-content: space-between;
}

.primary {
    width: 48%;
    height: 50px;
    display: flex;
    justify-content: center;
    font-size: 0.8rem;
}

.hidden {
    opacity: 0;
    visibility: hidden;
}
</style>

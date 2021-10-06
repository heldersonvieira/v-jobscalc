<template>
    <div class="input-box">
        <label for="input">
            {{ label }}
        </label>
        <input id="input" type="text" :placeholder="placeholder" />
    </div>
</template>

<script>
export default {
    props: {
        label: { type: String },
        placeholder: { type: String },
    },
};
</script>

<style scoped>
.input-box {
    display: flex;
    flex-direction: column;
    justify-content: flex-end;
}
label {
    font-size: 1.2rem;
    color: var(--text-gray);
}

input {
    width: 100%;
    height: 60px;
    padding: 1rem;
    margin-top: 1rem;
    border: none;
    border-radius: 5px;
    font-size: 1rem;
    color: var(--text-gray);
    outline: none;
}

#input::placeholder {
    color: var(--text-light-gray);
}
</style>

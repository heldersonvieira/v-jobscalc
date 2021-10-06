<template>
    <div class="profile__avatar">
        <nav class="profile__name">
            <h3>Jaqueline</h3>
            <router-link to="/profile">Ver perfil</router-link>
        </nav>
        <Avatar />
    </div>
</template>

<script>
import { Avatar } from '@/components';
export default {
    components: { Avatar },
};
</script>

<style scoped>
.profile__avatar {
    display: flex;
    align-items: center;
    gap: 1.5rem;
    color: var(--box);
}

.profile__name {
    text-align: right;
}

.avatar {
    width: 75px;
}

a {
    font-size: 0.9rem;
    line-height: 2rem;
    color: var(--text-light-gray);
    transition: all 0.3s ease;
}

a:hover {
    color: var(--orange);
    text-decoration: underline;
}
</style>

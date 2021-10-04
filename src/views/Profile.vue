<template>
    <div class="profile">
        <HeaderSubpage subtitle="Meu perfil" route="Home" />
        <ProfileCard />
    </div>
</template>

<script>
import { HeaderSubpage, ProfileCard } from '@/components';

export default {
    components: { HeaderSubpage, ProfileCard },
};
</script>

<style scoped></style>

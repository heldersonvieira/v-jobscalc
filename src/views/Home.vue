<template>
    <div class="header">
        <HeaderHome />
        <Container>
            <ul class="jobs-list">
                <JobInfoItem />
                <JobInfoItem />
                <JobInfoItem />
                <JobInfoItem />
                <JobInfoItem />
            </ul>
        </Container>
        <Modal />
    </div>
</template>

<script>
import { HeaderHome, Container, JobInfoItem, Modal } from '@/components';
export default {
    components: { HeaderHome, Container, JobInfoItem, Modal },
};
</script>

<style scoped>
.container {
    position: relative;
    top: -50px;
}

.jobs-list {
    padding: 0;
}
</style>

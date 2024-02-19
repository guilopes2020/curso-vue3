<template>
    <div>
        <img :src="avatar" :alt="description" width="350">
        <Reultilizacao />
    </div>
</template>

<script>
import Reultilizacao from './Reultilizacao.vue';
    export default {
        name: 'Picture',
        data() {
            return {
                avatar: '/img/avatar.jpg',
                description: 'corsa'
            }
        },
        components: {
            Reultilizacao
        }
    }
</script>
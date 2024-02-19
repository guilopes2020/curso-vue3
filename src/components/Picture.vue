<template>
    <div>
        <img :src="avatar" :alt="description" width="350">
        <MudarImagem @mudar-imagem="trocarImagem" />
    </div>
</template>

<script>
import Reultilizacao from './Reultilizacao.vue';
import MudarImagem from './MudarImagem.vue';
    export default {
        name: 'Picture',
        data() {
            return {
                avatar: '/img/avatar.jpg',
                description: 'corsa'
            }
        },
        methods: {
            trocarImagem() {
                if (this.avatar == '/img/avatar.jpg') {
                    this.avatar = '/img/avatar2.jpg'
                } else {
                    this.avatar = '/img/avatar.jpg'
                }
            }
        },
        components: {
            Reultilizacao,
            MudarImagem
        }
    }
</script>
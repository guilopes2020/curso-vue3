<template>
    <div>
        <p v-if="esta_trabalhando">Estou trabalhando no momento</p>
        <p v-else>estou desempregado</p>
        <p>ultilizo as seguintes tecnologias:</p>
        <ul>
            <li>Javascript</li>
            <li>PHP</li>
            <li>Phyton</li>
        </ul>
        <p v-show="mostrar_email">mande uma mensagem para: {{ email }}</p>
        <p>Para acessar meu portifolio <a v-bind:href="meu_link" target="_blank">basta clicar aqui</a></p>
        <Picture />
    </div>
</template>

<script>
import Picture from './Picture.vue';
    export default {
        name: 'Info',
        components: {
            Picture
        },
        data() {
            return {
                esta_trabalhando: true,
                mostrar_email: true,
                email: 'jdhfjdhfd@gmail.com',
                meu_link: 'https://google.com'
            }
        }
    }
</script>
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
        <div>
            <button @click="showEmail">{{ texto_botao }}</button>
        </div>
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
                mostrar_email: false,
                email: 'jdhfjdhfd@gmail.com',
                meu_link: 'https://google.com',
                texto_botao: 'mostrar email'
            }
        },
        methods: {
            showEmail() {
                this.mostrar_email = !this.mostrar_email
                if (!this.mostrar_email) {
                    this.texto_botao = 'mostrar email'
                } else {
                    this.texto_botao = 'ocultar email'
                }
            }
        }
    }
</script>
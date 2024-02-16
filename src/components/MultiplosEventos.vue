<template>
    <div>
        <button @click="primeiro(txt1, $event), segundo(txt2, $event), terceiro(txt3, $event), limpar()">ativar multiplos eventos</button>
        <p>{{ multiplos_eventos }}</p>
    </div>
</template>

<script>
    export default {
        name: 'MultiplosEventos',
        data() {
            return {
                multiplos_eventos: '',
                txt1: 'primeiro evento ativado!',
                txt2: 'segundo evento ativado',
                txt3: 'terceiro evento ativado'
            }
        },
        methods: {
            primeiro(texto, e) {
                this.multiplos_eventos = texto
            },
            segundo(texto, e) {
                setTimeout(() => {
                    this.multiplos_eventos = texto
                }, 1000)
            },
            terceiro(texto, e) {
                setTimeout(() => {
                    this.multiplos_eventos = texto
                }, 2000)
            },
            limpar(e) {
                setTimeout(() => {
                    this.multiplos_eventos = ''
                }, 3000)
            }
        }
    }
</script>

<style scoped>
    div {
        margin: 100px;
    }
</style>
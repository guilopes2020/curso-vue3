<template>
    <div>
        <h1>Olá Vue!</h1>
        <p>meu nome é: {{ nome }}, tenho {{ age }} anos de idade e sou {{ profissao }}</p>
        <MultiplosEventos />
    </div>
</template>

<script>
import MultiplosEventos from './MultiplosEventos.vue';
    export default {
        name: 'PrimeiroComponente',
        components: {
            MultiplosEventos
        },
        data() {
            return {
                nome: 'Matheus',
                profissao: 'programador',
                age: 27
            }
        }
    }
</script>
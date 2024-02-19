<template>
    <div>
        <Reultilizacao />
        <h1>Olá Vue!</h1>
        <Reultilizacao />
        <p>meu nome é: {{ nome }}, tenho {{ age }} anos de idade e sou {{ profissao }}</p>
        <Reultilizacao />
        <MultiplosEventos />
        <Reultilizacao />
        <Reultilizacao />
        <Reultilizacao />
        <Reultilizacao />
    </div>
</template>

<script>
import MultiplosEventos from './MultiplosEventos.vue';
import Reultilizacao from './Reultilizacao.vue';
    export default {
        name: 'PrimeiroComponente',
        components: {
            MultiplosEventos,
            Reultilizacao
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
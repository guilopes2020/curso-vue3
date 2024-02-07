<template>
    <div>
        <h1>Olá Vue!</h1>
        <p>meu nome é: {{ nome }}, tenho {{ age }} anos de idade e sou {{ profissao }}</p>
    </div>
</template>

<script>
    export default {
        name: 'PrimeiroComponente',
        data() {
            return {
                nome: 'Matheus',
                profissao: 'programador',
                age: 27
            }
        }
    }
</script>
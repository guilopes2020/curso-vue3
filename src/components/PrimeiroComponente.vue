<template>
    <div>
        <h1>Olá Vue!</h1>
        <p>meu nome é: {{ name }}, tenho {{ age }} anos de idade e sou {{ profissao }}</p>
    </div>
</template>

<script>
    export default {
        name: 'PrimeiroComponente',
        data() {
            return {
                name: 'Matheus',
                profissao: 'programador',
                age: 27
            }
        }
    }
</script>
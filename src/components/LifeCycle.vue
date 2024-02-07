<template>
    <div>
        <h1>meu nome é: {{ nome }}</h1>
    </div>
</template>

<script>
    export default {
        name: 'LifeCycle',
        data() {
            return {
                nome: 'ainda nao sei'
            }
        },
        created() {
            setTimeout(() => {
                this.nome = 'Guillherme'
            }, 2000)
        },
        mounted() {
            setTimeout(() => {
                this.nome = 'Pedro'
            }, 4000)
        }
    }
</script>
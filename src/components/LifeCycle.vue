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
            this.lifeCycle()
        },
        mounted() {
            setTimeout(() => {
                this.nome = 'Pedro'
            }, 4000)
        },
        methods: {
            lifeCycle() {
                console.log('executou lifecycle')
            }
        }
    }
</script>
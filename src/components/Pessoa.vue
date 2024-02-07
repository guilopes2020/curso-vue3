<template>
    <div>
        <h2>esta é a descrição da pessoa {{ nome }}</h2>
        <Info />
        <Form />
    </div>
</template>

<script>
import Info from './Info'
import Form from './Form.vue';
    export default {
        name: 'Pessoa',
        data() {
            return {
                nome: 'Ana',
                description: 'alta e morena'
            }
        },
        components: {
            Info,
            Form
        }
    }
</script>
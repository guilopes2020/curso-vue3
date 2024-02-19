<template>
    <div>
        <h2>esta é a descrição da pessoa {{ nome }}</h2>
        <Info :email="email" :esta_trabalhando=true />
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
                description: 'alta e morena',
                email: 'gregreg@fdkfgdfk.com'
            }
        },
        components: {
            Info,
            Form
        }
    }
</script>
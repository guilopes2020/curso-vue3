<template>
    <div>
        <form action="" @submit="enviarForm($event)">
            <div>
                <input type="text" v-model="name">
            </div>
            <div>
                <input type="text" v-model="email">
            </div>
            <div>
                <Submit />
            </div>
        </form>
    </div>
</template>

<script>
import InputText from './form/InputText.vue'
import Submit from './form/Submit.vue'
    export default {
        name: 'Form',
        components: {
            InputText,
            Submit
        },
        data() {
            return {
                name: '',
                email: ''
            }
        },
        methods: {
            enviarForm(e) {
                e.preventDefault()
                const name = this.name
                const email = this.email
                console.log(`o nome é ${name} e o email é ${email}`)
            }
        }
    }
</script>
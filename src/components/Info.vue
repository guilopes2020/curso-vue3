<template>
    <div>
        <p v-if="esta_trabalhando">Estou trabalhando no momento</p>
        <p v-else>estou desempregado</p>
        <p>ultilizo as seguintes tecnologias:</p>
        <ul>
            <li>Javascript</li>
            <li>PHP</li>
            <li>Phyton</li>
        </ul>
        <p v-show="mostrar_email">mande uma mensagem para: {{ email }}</p>
    </div>
</template>

<script>
    export default {
        name: 'Info',
        data() {
            return {
                esta_trabalhando: true,
                mostrar_email: true,
                email: 'jdhfjdhfd@gmail.com'
            }
        }
    }
</script>
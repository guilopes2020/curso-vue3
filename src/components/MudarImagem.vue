<template>
    <div>
        <button @click="$emit('mudarImagem')">trocar imagem</button>
    </div>
</template>

<script>
    export default {
        name: 'MudarImagem',
        emits: ['mudarImagem']
    }
</script>
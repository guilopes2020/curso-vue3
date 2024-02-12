<template>
    <div>
        <img :src="avatar" :alt="description" width="350">
    </div>
</template>

<script>
    export default {
        name: 'Picture',
        data() {
            return {
                avatar: '/img/avatar.jpg',
                description: 'corsa'
            }
        }
    }
</script>
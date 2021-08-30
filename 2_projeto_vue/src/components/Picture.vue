<template>
    <div>
        <Reutilizacao />
        <img :src="avatar" :alt="descricao">
    </div>
</template>

<script>
import Reutilizacao from './Reutilizacao.vue'
export default {
    name: 'Picture',
    components: {
        Reutilizacao
    },
    data() {
        return {
            avatar: "/img/avatar.png",
            descricao: "Henington Frota"
        }
    },
}
</script>

<style>

</style>
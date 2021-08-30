<template>
    <div>
        <img :src="avatar" :alt="descricao" width="100">
        <MudarImagem @mudar-imagem="trocarImagem" />
    </div>
</template>

<script>
import MudarImagem from './MudarImagem.vue'
export default {
    name: 'Picture',
    components: {
        MudarImagem
    },
    data() {
        return {
            avatar: "/img/avatar.png",
            descricao: "Henington Frota"
        }
    },
    methods: {
        trocarImagem() {
            this.avatar = "/img/avatar2.png"
        }
    },
}
</script>

<style>

</style>
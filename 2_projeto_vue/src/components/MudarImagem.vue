<template>
    <div>
        <button @click="$emit('mudarImagem')">Trocar Imagem Perfil</button>
    </div>
</template>

<script>
export default {
    name: 'MudarImagem',
    emits: ['mudarImagem']
}
</script>

<style>

</style>
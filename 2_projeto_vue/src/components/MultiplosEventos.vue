<template>
    <div>
        <button @click='primeiro("Primeiro Evento!", $event), segundo("Segundo Evento!", $event), terceiro()'>Ativar Multiplos Eventos</button>
        <p>{{ multiplos_eventos }}</p>
    </div>
</template>

<script>
export default {
    name: 'MultiplosEventos',
    data() {
        return {
            multiplos_eventos: ""
        }
    },
    methods: {
        primeiro(txt, e) {
            this.multiplos_eventos = txt;
        },
        segundo(txt, e) {
            setTimeout(() => this.multiplos_eventos = txt, 500);
        },
        terceiro(txt, e) {
            setTimeout(() => this.multiplos_eventos = "", 1500);
        }
    },
}
</script>

<style scoped>
    div {
        padding: 100px;
        border: 1px solid #fff;
    }
</style>
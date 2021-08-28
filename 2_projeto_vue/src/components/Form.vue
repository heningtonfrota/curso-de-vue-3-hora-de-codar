<template>
    <form action="" @submit="enviarFormulario($event)">
        <h2>Meu Formulário: </h2>
        <div>
            <input type="text" v-model="name">
        </div>
        <div>
            <input type="text" v-model="email">
        </div>
        <div>
            <Submit />
        </div>
        <p>Conteudo</p>
        <p>Conteudo</p>
        <p>Conteudo</p>
        <p>Conteudo</p>
    </form>
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
        enviarFormulario(e) {
            e.preventDefault();

            const name = this.name;
            const email = this.email;
            console.log('Formulario Enviado!');
            console.log('Nome é: ' + this.name);
            console.log('E-mail é: ' + this.email);
        }
    },
}
</script>

<style scoped>
    p {
        margin: 80px;
    }
</style>
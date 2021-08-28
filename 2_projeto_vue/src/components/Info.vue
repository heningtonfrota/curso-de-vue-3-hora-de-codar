<template>
    <div>
        <p v-if="esta_trabalhando">Estou trabalhando no momento.</p>
        <p v-else>Estou em busca de novas oportunidades.</p>
        <p>Utilizo as seguintes tecnologias para beck-end: </p>
        <ul>
            <li v-for="(tecnologia, index) in beckend_tecnologia" :key="index">
                {{ tecnologia }}
            </li>
        </ul>
        <p>Utilizo as seguintes tecnologias para front-end: </p>
        <ul>
            <li v-for="tecnologia in frontend_tecnologia" :key="tecnologia.id">
                {{ tecnologia.linguagem }}
            </li>
        </ul>
        <div>
            <button @click="showEmail">{{ texto_botao }}</button>
        </div>
        <p v-show="mostrar_email">Mande uma mensagem para: {{ email }}</p>
        <p class="teste">Para acessar meu portifolio basta <a v-bind:href="meu_link" target="_blank">Clicar Aqui</a></p>
        <Picture />
    </div>
</template>

<script>
import Picture from './Picture.vue'
export default {
    name: 'Info',
    components: {
        Picture
    },
    data() {
        return {
            esta_trabalhando: true,
            mostrar_email: false,
            email: 'heningtonfrota@gmail.com',
            meu_link: 'https://google.com',
            texto_botao: 'Mostrar e-mail',
            beckend_tecnologia: [
                'JavaScript',
                'PHP',
                'Python'
            ],
            frontend_tecnologia: [
                {id: 1, linguagem: 'HTML'},
                {id: 2, linguagem: 'CSS'},
                {id: 3, linguagem: 'Vue'},
            ]
        }
    },
    methods: {
        showEmail(){
            this.mostrar_email = !this.mostrar_email
            if (!this.mostrar_email) {
                this.texto_botao = "Mostrar e-mail"
            } else { 
                this.texto_botao = "Ocultar e-mail"
            }
        }
    },
}
</script>

<style>
    .paragrafo-pai {
        color: red;
    }
</style>
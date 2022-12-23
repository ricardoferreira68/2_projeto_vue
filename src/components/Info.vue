<template>
    <div>
        <p v-if="esta_trabalhando">Estou trabalhando no momento.</p>
        <p v-else>Estou em busca de novas oportunidades.</p>
        <p>Utilizo as seguintes tecnologias de frontend:</p>
        <ul>
            <li v-for="(technology, index) in frontend_technologies" v-bind:key="index">
                {{ technology }}
            </li>
        </ul>  
        <p>Utilizo as seguintes tecnologias de backend:</p>
        <ul>
            <li v-for="technology in backend_technologies" v-bind:key="technology.id">
                {{ technology.technology }}
            </li>
        </ul>  
        <div>
            <button @click="showEmail">
                <span v-if="mostrar_email">Acultar e-mail</span>
                <span v-else>Mostar e-mail</span>
            </button>
        </div>
        <p v-show="mostrar_email">Mande uma mensagem para: {{ email }}</p>
        <p class="menssage">Para acessar o meu portfólio <a v-bind:href="meu_link" target="_blank">basta clicar aqui</a></p>
        <Picture />
    </div>
</template>

<script>
import Picture from './Form/Picture.vue';

export default {
    name: "Info",
    components: {
        Picture,
    },
    data() {
        return {
            esta_trabalhando: false,
            mostrar_email: false,
            email: "jrsf68@gmail.com",
            meu_link: "https://google.com",
            frontend_technologies: ['HTML', 'CSS', 'JavaScript', 'Vue.js', 'Yew'],
            backend_technologies: [
                {id: 1, technology: 'Python'}, 
                {id: 2, technology: 'JavaScript'}, 
                {id: 3, technology: 'Rust'}, 
                {id: 4, technology: 'PHP'},
            ],
        };
    },
    methods: {
        showEmail() {
            this.mostrar_email = !this.mostrar_email;
        }
    },
}
</script>

<style>
    .titulo {
        font-size: 40px;
        font-weight: bold;
    }
</style>
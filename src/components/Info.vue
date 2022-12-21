<template>
    <div>
        <p v-if="esta_trabalhando">Estou trabalhando no momento.</p>
        <p v-else>Estou em busca de novas oportunidades.</p>
        <p>Utilizo as seguintes tecnologias:</p>
        <ul>
            <li>Python</li>
            <li>JavaScript</li>
            <li>Node.js</li>
            <li>Vue.js</li>
            <li>Rust</li>
            <li>Tokio</li>
            <li>Yew</li>
        </ul>  
        <p v-show="mostrar_email">Mande uma mensagem para: {{ email }}</p>
        <p>Para acessar o meu portfólio <a v-bind:href="meu_link" target="_blank">basta clicar aqui</a></p>
        <div>
            <button></button>
        </div>
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
        };
    },
}
</script>
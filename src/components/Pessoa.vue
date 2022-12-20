<template lang="">
    <div>
        <h2>Esta é a descricao da pessoa: {{ nome }}</h2>
        <p>Estou trabalhando no momento</p>
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
    </div>
</template>
<script>
export default {
    name: 'Pessoa',
    data() {
        return {
            nome: 'Ricardo'
        }
    },
}
</script>
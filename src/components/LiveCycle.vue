<template>
    <div>
        <h1>Olá Vue!</h1>
        <p>Meu nome é {{ name }} e sou {{ profissao }}</p>    
    </div>
</template>

<script>
    export default {
        name: 'LiveCycle',
        data() {
            return{
                name: "Ciclo de Vida",
                profissao: "dev",
            }
        },
        created() {
            setTimeout(() => {
                this.name = 'Gabriela'
            }, 1000);
        },
        mounted() {
            setTimeout(() => {
                this.name = 'Rafinha'
            }, 2000);
        },
    }
</script>
<template>
    <div>
        <img :src="avatar" :alt="descricao">
    </div>
</template>

<script>
export default {
    nome: 'Picture',
    data() {
        return {
            avatar: "/img/icone_usuario_sem_fundo.png",
            descricao: "Ícone de usuário",
            
        }
    }
}
</script>

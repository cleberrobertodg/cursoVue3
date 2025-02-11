<template>
    <div>
        <img :src="avatar" :alt="descricao" >
        <MudarImagem @mudar-imagem="trocarImagem"/>
    </div>
</template>

<script>
import MudarImagem from './MudarImagem.vue';
    export default{
        name: 'Picture',
        components: {
            MudarImagem
        },
        data(){
            return{
                avatar: "https://raw.githubusercontent.com/matheusbattisti/curso_vue_yt/refs/heads/main/9_argumentos/public/img/avatar.png",
                descricao: "Boneco"
            }
        },
        methods: {
            trocarImagem(){
                this.avatar = "https://raw.githubusercontent.com/matheusbattisti/curso_vue_yt/refs/heads/main/17_emit/public/img/avatar2.png"
            }
        }
    }
</script>
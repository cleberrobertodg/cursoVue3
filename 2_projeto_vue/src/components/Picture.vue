<template>
    <div>
        <img :src="avatar" :alt="descricao" >
    </div>
</template>

<script>
    export default{
        name: 'Picture',
        data(){
            return{
                avatar: "https://raw.githubusercontent.com/matheusbattisti/curso_vue_yt/refs/heads/main/9_argumentos/public/img/avatar.png",
                descricao: "Boneco"
            }
        }
    }
</script>
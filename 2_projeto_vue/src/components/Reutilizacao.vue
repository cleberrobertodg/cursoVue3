<template>
    <div>
        <button @click="ativar_mensagem">Clique aqui!</button>
        <span v-show="ativou">Ativado</span>
    </div>
</template>

<script>
export default {
    name: "Reutilizacao",
    data(){
        return{
            ativou: false
        }
    }, 
    methods: {
        ativar_mensagem(){
            this.ativou = !this.ativou
        }
    }
}
</script>
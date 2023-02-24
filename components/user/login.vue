<template>
    <v-card class="cardLogin">
        <v-card-title>Login</v-card-title>
        <v-card-text>
            <v-form v-model="formularioValido">
                <v-text-field label="Correo Electronico" 
                placeholder="Correo Electronico"
                v-model="correoElectronico"/>
            </v-form>
        </v-card-text>
        <v-card-actions>
            Boton para iniciar sesion
        </v-card-actions>
    </v-card>
</template>

<script>
export default {
    data() {
        return {
            formularioValido: false,
            correoElectronico: ''
        }
    }
}
</script>

<style scoped>   
/* se pone siempre scoped para dar un unico estilo ala pagina */

/* a qui ponemos los estilos ala pagina */
.cardLogin {
    background-color: crimson;
    border-radius: 10px;
    width: 500px;
    height: 300px;
}
</style>
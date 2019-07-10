<template>
    <div>
        
        <div class="header">
            <div class="teste"><img src="../../assets/images/movies.png" class="img"></div>
            <div class="body-login">
                <table cellspacing="0" role="presentation">
                    <tbody>
                        <tr>
                            <td><DInput :label="'E-mail'"/></td>
                            <td><DInput :label="'Senha'"/></td>
                            <td><a-button class="btn-login" type="primary">Entrar</a-button></td>
                        </tr>
                        
                        <tr>
                            <div>
                                <a href="#" class="link">Esqueceu a conta?</a>
                            </div>
                        </tr>
                    </tbody>
                </table>

            </div>
        </div>

        <div class="content">

            <div class="new-account">
                <DInput :label="'Nome'"/>
                <DInput :label="'Sobrenome'"/>
                <DInput :addStyle="'double'" :classDiv="'double-div'" :label="'E-mail'"/>
                <DInput :label="'Senha'"/>
                <DInput :label="'Confirmar senha'"/>
                <DInput :addStyle="'double'" :classDiv="'double-div'" :label="'Data de nascimento'"/>
                <a-button class="btn-create-user" type="primary">Criar Conta</a-button>
            </div>

        </div>
        <div class="footer">

        </div>
    </div>
</template>

<script>

import DInput from '../../components/Input/Input.vue';
import DButton from '../../components/Button/Button.vue';

export default {
  name: 'Login',
  data(){
    return{}
  },
  props: {
    msg: String
  },
  components: {
    DInput,
    DButton,
    // HelloWorld
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
@import './Login.css';
</style>

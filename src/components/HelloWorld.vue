<template>
  <table cellspacing="0" role="presentation">
    <tbody>
      <tr>
        <td class="html7magic">
          <label for="email">Email ou telefone</label>
        </td>
        <td class="html7magic">
          <label for="pass">Senha</label>
        </td>
      </tr>

      <tr>
        <td>
          <input type="email" class="inputtext" name="email" id="email" data-testid="royal_email">
        </td>
        <td>
          <input type="password" class="inputtext" name="pass" id="pass" data-testid="royal_pass">
          </td>
        <td>
          <label class="uiButton uiButtonConfirm" id="loginbutton" for="u_0_2">
            <input value="Entrar" aria-label="Entrar" data-testid="royal_login_button" type="submit" id="u_0_2">
          </label>
        </td>
      </tr>
      
      <tr>
        <td class="login_form_label_field">
          <div>
            <a href="https://www.facebook.com/recover/initiate?lwv=110&amp;ars=royal_blue_bar">Esqueceu a conta?</a>
          </div>
        </td>
      </tr>
    </tbody>
  </table>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>

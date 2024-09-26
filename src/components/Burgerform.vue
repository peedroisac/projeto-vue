<template>
  <div>
    <p>componente de mensagem</p>
    <div>
      <form id="burger-form">
        <div class="input-container">
          <label for="nome">Nome do Cliente</label>
          <input type="text" id="nome" name="nome" v-model="nome" placeholder="digite seu nome" />
        </div>
        <div class="input-container">
          <label for="pao">Escolha o pão:</label>
          <select name="pao" id="pao" v-model="pao">
            <option value="">Selecione o seu pão</option>
            <option value="">integral</option>
          </select>
        </div>
        <div class="input-container">
            <label for="carne">Escolha a carne do seu burger:</label>
            <select name="carne" id="carne" v-model="carne">
              <option value="">Selecione sua carne</option>
              <option value="">maminha</option>
            </select>
        </div>
        <div class="input-container">
          <label for="opicionais">Selecione os opcionais:</label>
          <input type="checkbox" name="opicionais" v-model="opicionais" value="salame">
            <span>Salame</span>
        </div>
      </form>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Burgerform',
}
</script>

<style scoped>
</style>
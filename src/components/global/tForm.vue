<template>
<form class="form">
  <h2 class="form-header">Регистрация</h2>
  <div class="form-auth">
    <p class="form-auth-text">Уже есть аккаунт?</p><a class="form-auth-link" href="#">Войти</a>
  </div>
  <label class="label-text">Имя</label>
  <t-input class="form-input" placeholder="Введите имя"/>
  <label class="label-text" >Email</label>
  <t-input class="form-input" placeholder="Введите ваш email"/>
  <label class="label-text">Номер телефона</label>
  <t-input class="form-input" placeholder="Введите ваш номер телефона"/>
  <label class="label-text">Язык</label>
  <t-select class="form-select"/>
  <div class="form-agreement">
    <t-checkbox/><p>Принимаю <a>условия</a> использования</p>
  </div>
  <t-button value="Зарегистрироваться" :is-active="btnActive"/>
</form>
</template>

<script>
import TInput from "@/components/ui/tInput";
import TButton from "@/components/ui/tButton";
import TSelect from "@/components/ui/tSelect";
import TCheckbox from "@/components/ui/tCheckbox";
export default {
  name: "tForm",
  components: {TCheckbox, TSelect, TButton, TInput},
  data(){
    return {
      btnActive: true
    }
  }
}
</script>

<style scoped>
.form {
  display: flex;
  flex-direction: column;
  width: 398px;
  /*height: 789px;*/
  padding: 40px 30px;
  border-radius: 24px;
  border: solid 1px #DBE2EA;
}
.label-text,
.label-header {
  display: flex;
  align-items: flex-start;
}

.label-header {
  color: #2C2738;
  font-size: 34px;
  font-weight: bold;
  margin-bottom: 9px;
}

.form-auth {
  display: flex;
  flex-direction: row;
  margin-bottom: 53px;
  font-size: 16px;
  font-weight: normal;
}

.form-auth-text {
  padding: 0;
  margin: 0 10px 0 0;
}

a {
  color: #0880AE;
  text-decoration: none;
}

.label-text {
  color: #756F86;
  margin-bottom: 8px;
}

.form-input {
  margin-bottom: 34px;
}

.form-select {
  margin-bottom: 32px;
}

.form-agreement {
  font-weight: 500;
  display: flex;
  text-align: center;
}

p {
  margin: 0;
}
</style>

<template>
  <form dir="rtl" class="form">
    <div class="container">
      <v-row class="input-row">
        <div class="input-container title-text">התחברות</div>
      </v-row>
      <v-row class="input-row">
        <div class="input-container">
          <label> שם משתמש </label>
          <v-text-field
            class="text-field"
            v-model="userName"
            outlined
            dense
          ></v-text-field>
        </div>
      </v-row>
      <v-row class="input-row">
        <div class="input-container">
          <label> סיסמה </label>
          <v-text-field
            type="password"
            outlined
            dense
            class="text-field"
            v-model="password"
          ></v-text-field>
        </div>
      </v-row>
      <v-row class="input-row">
        <div class="input-container">
          <v-checkbox
            color="purple"
            v-model="rememberMe"
            label="זכור אותי"
          ></v-checkbox>
        </div>
      </v-row>
      <v-row class="input-row">
        <div class="input-container">
          <v-btn
            color="rgba(118, 3, 128, 0.83)"
            class="button input-row"
            dark
            @click="submit"
          >
            התחברות
          </v-btn>
        </div>
      </v-row>
    </div>
  </form>
</template>

<script>
export default {
  name: "LoginForm",

  data: () => ({
    rememberMe: false,
    userName: null,
    password: null,
  }),
};
</script>
<style scoped>
.input-row {
  justify-content: center;
  padding: 0;
  font-size: 18px;
}
.button {
  background: rgba(118, 3, 128, 0.83);
  mix-blend-mode: normal;
  border-radius: 10px;
}
.text-field {
  border-radius: 10px;
}
.column {
  padding: 0;
}
.form {
  margin: 20vh;
}
.input-container {
  display: flex;
  flex-direction: column;
  width: 100%;
}
.container {
  width: 22vw;
}
.title-text {
  margin-bottom: 20px;
  font-size: 28px;
  font-family: "Varela Round";
}
</style>

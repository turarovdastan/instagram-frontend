<template>
<v-container>
<v-img height="200" src="https://cdn.vuetifyjs.com/images/cards/server-room.jpg"></v-img>

    <form class="mt-5" @submit.prevent="submit">
        <v-text-field
          v-model="email"
          label="E-mail"
          required
          solo
          type="email"
        ></v-text-field>
        <v-text-field
          v-model="password"
          label="password"
          required
          solo
          type="password"
        ></v-text-field>
      <v-btn
        class="mr-4 col-12"
        type="submit"
        :disabled="invalid"
      >
        Login
      </v-btn>
    </form>
</v-container>
</template>


<script>



  export default {
    data: () => ({
      email: '',
      password:''
    }),

    methods: {
      submit () {
      },
    },
  }
</script>
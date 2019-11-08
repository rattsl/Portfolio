<template>
  <v-app class="grey lighten-4">
      <v-container>
      <v-row
      align="center"
      justify="center"
      >
        <h1 class="display-3 font-weight-bold ul my-12 d-inline-block">Contact</h1>
      </v-row>
      <v-row
        align="center"
        justify="center"      
      >
          <form>
            <v-text-field
            v-model="name"
            :error-messages="nameErrors"
            :counter="10"
            label="Name"
            required
            @input="$v.name.$touch()"
            @blur="$v.name.$touch()"
            max-width="700"
            ></v-text-field>
            <v-text-field
            v-model="email"
            :error-messages="emailErrors"
            label="E-mail"
            required
            @input="$v.email.$touch()"
            @blur="$v.email.$touch()"
            ></v-text-field>
            <v-textarea
            name="input-7-1"
            label="Default style"
            value="The Woodman set to work at once, and so sharp was his axe that the tree was soon chopped nearly through."
            hint="Hint text"
            ></v-textarea>
            <v-checkbox
            v-model="checkbox"
            :error-messages="checkboxErrors"
            label="Do you agree?"
            required
            @change="$v.checkbox.$touch()"
            @blur="$v.checkbox.$touch()"
            ></v-checkbox>

            <v-btn class="mr-4" @click="submit">submit</v-btn>
            <v-btn @click="clear">clear</v-btn>
        </form>
      </v-row>
      </v-container>
  </v-app>
</template>

<script>
export default {

}
</script>

<style>

</style>
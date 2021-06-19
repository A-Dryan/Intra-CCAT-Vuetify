<template>
    <v-container 
    style="width: 750px;
           height: 100vh;
           display: flex"
    justify="center"
    align="center">
    <v-row align="center" justify="center">
       <v-col
      cols="12"
      sm="10"
      md="8"
      lg="6"
    >
    <v-card ref="form" class="elevation-10">
        <v-img
              src="https://lh3.googleusercontent.com/proxy/3S6hdnfvcgiYWSEz0FFOCcM62vFNlOBGgLjHpL-0IWDuOfPUb3C0eQd-0c6t4LQw1eX_vvJKOQzZOBeETmyYkbFLjaYFHonWA-e2WkGe5Dvv00FySXZVDxvPQhluE3lk"
              height="300"
              contain
            ></v-img>
            <v-card-title class="text-h6">
              LOGIN
            </v-card-title>
        <v-card-text>
             <v-text-field
            ref="name"
            v-model="name"
            :rules="[() => !!name || 'This field is required']"
            :error-messages="errorMessages"
            label="Username"
            required
          ></v-text-field>
             <v-text-field
            v-model="password"
            name="Password"
            label="Password"
            type="password"
          ></v-text-field>
           <v-btn
           block
            class="mr-4"
            @click="submit"
            color="primary"
            to="/modHome">
             Sign in
            </v-btn>
        </v-card-text>
    </v-card>
       </v-col>
    </v-row>
  </v-container>
</template>
<template>

<q-page>

  <div class=" flex flex-center column col-6  q-pa-md">
          <q-img
          src="https://images.pexels.com/photos/9542697/pexels-photo-9542697.jpeg?auto=compress&cs=tinysrgb&h=750&w=1260"
          spinner-color="red"
          style="height: 200px; max-width: 200px; border-radius: 100%  "
          >
          </q-img>
          <div class="col-md-2 col-sm-2 items-center q-pa-md">
            <q-btn color="primary" label="Cambiar Foto" />
          </div>
        </div>
        <div class="col-6 q-pa-sm flex justify-center  ">
          <q-card class="my-card " style=" width: 35% ">
        <q-card-section class="column items-center flex justify-center">
          <p class="text-h6 text-weight-regular">Name</p>
          <p class="text-weight-regular" > {{this.name}} </p>
        </q-card-section>
      </q-card>

      <q-card class="my-card" style=" width: 35% ">
    <q-card-section class="column items-center flex justify-center	" >
    <p class="text-h6 text-weight-regular">Job</p>
    <p class="text-weight-regular" > {{this.job}} </p>
    <router-link to="/Update">
      <q-btn style="background: #FF0080; color: white; font-size: 11px;" label="Edit" />
    </router-link>
    </q-card-section>
  </q-card>

        </div>

  </q-page>


</template>

<script>
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'IndexPage',
  data(){
    return {
      name: "Robert",
      job: "Developer"
    }
  }
})
</script>

<style>



</style>

<template>
    <ion-input v-bind="$attrs" :type="type" :id="id" :value="value" :placeholder="placeholder" :clearInput="clearInput" :debounce="debounce" :disabled="disabled" :maxlength="maxlength" :min="min" :max="max" :step="step"></ion-input>
    <!-- <div>
      <div>Primer Nombre: {{ firstName }}</div>
      <div>Segundo Nombre: {{ middleName }}</div>
      <div>Primer Apellido: {{ lastName }}</div>
      <div>Segundo Apellido: {{ secondLastName }}</div>
      <div>Documento: {{ documentType }} - {{ documentNumber }}</div>
    </div>   -->
</template>
  
  <script lang="ts">
  import { IonInput } from '@ionic/vue';
  import { defineComponent } from 'vue';
  
  export default defineComponent({
    components: { IonInput },
    props: {
      type: String,
      id: {
        type: String,
        required: true
      },name: String,
      value: String,
      aceholder: String,
      clearInput: Boolean,
      debounce: Number,
      disabled: Boolean,
      maxlength: Number,
      min: Number,
      max: Number,
      step: Number,
      placeholder: String,
      //----------->
      firstName: String,
      middleName: String,
      lastName: String,
      secondLastName: String,
      documentType: String,
      documentNumber: String
    }
  });
  </script>
  
  <style scoped>
  /* Estilos del componente */
  /* Estilos globales */
  </style>
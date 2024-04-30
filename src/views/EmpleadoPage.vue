<template>
    <ion-page>
      <ion-header :translucent="true">
        <ion-toolbar>
          <ion-title>Empleado</ion-title>
        </ion-toolbar>
      </ion-header>  
      <ion-content>       
        <div id="login-container">  
          <div id="login-form">           
            <PersonaComponent id="primerNombre" name="primerNombre" label="Primer nombre: " />
            <PersonaComponent id="segundoNombre" name="segundoNombre" label="Segundo nombre: " />
            <PersonaComponent id="primerApellido" name="primerApellido" label="Primer apellido: " />
            <PersonaComponent id="segundoApellido" name="segundoApellido" label="Segundo apellido: " />
            <PersonaComponent type="number" id="Documento" name="Documento" label="Documento: " />
            <PersonaComponent id="id" name="id" type="hidden"/>
          </div>
  
          <div> 
             <!--Traer el componente de los botones de la crud  -->
            <CrudButtonComponent />
          </div>          
        </div>
      </ion-content>
    </ion-page>
  </template>
  
  <script setup lang="ts">
  import { IonContent, IonHeader, IonPage, IonTitle, IonToolbar } from '@ionic/vue';
  
  import CrudButtonComponent from '@/components/CrudButtonComponents.vue';
  import PersonaComponent from '@/components/PersonaComponent.vue';
  </script>
  
  <style scoped src="../theme/container.css"></style>

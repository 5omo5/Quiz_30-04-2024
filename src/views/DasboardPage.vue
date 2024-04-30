<template>
    <ion-page>
      <ion-header :translucent="true">
        <ion-toolbar>
          <ion-title>Dashboard</ion-title>
        </ion-toolbar>
      </ion-header>
  
      <ion-content>
        <br>
        <ion-content id="container">
          <strong><a href="/cliente" class="boton">Ir a Clientes</a></strong>          
          <br>
          <strong><a href="/producto" class="boton">Ir a productos</a></strong>
          <br>
          <strong><a href="/otrocliente" class="boton">Ir a otro cliente</a></strong>
          <br>
          <strong><a href="/empleado" class="boton">Ir a Empleado</a></strong>
          <br>
          <strong><a href="/estudiante" class="boton">Ir a Estudiante</a></strong>
          <br>
  
        </ion-content>div>
  
      </ion-content>
    </ion-page>
  </template>
  
  <script setup lang="ts">
  import { IonContent, IonHeader, IonPage, IonTitle, IonToolbar } from '@ionic/vue';
  </script>
  
  <style scoped>
.boton {
  display: block;
  padding: 10px 30%;
  background-color: #007bff; /* Azul */
  color: #ffffff; /* Texto blanco */
  text-decoration: none; /* Quitar subrayado */
  border-style: outset;
  border-radius: 5px;
  cursor: pointer;
}

.boton:hover {
  background-color: #0056b3; /* Azul más oscuro al pasar el ratón */
}

</style>
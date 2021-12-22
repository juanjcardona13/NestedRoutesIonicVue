<template>
  <ion-page id="WizardLayout">
    <ion-header class="ion-no-border">
      <ion-toolbar>
        <ion-buttons slot="start">
          <ion-back-button color="dark" default-href="/tabs/tab1" @click="() => $router.push('/tabs/tab1')" text="" :icon="arrowBackOutline">
          </ion-back-button>
        </ion-buttons>
        <ion-title>{{tituloHeader}}</ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content class="ion-padding">
      <ion-router-outlet />
    </ion-content>
  </ion-page>
</template>

<script>
import {
    IonPage,
    IonHeader,
    IonToolbar,
    IonButtons,
    IonBackButton,
    IonTitle,
    IonContent,
    IonRouterOutlet,
} from "@ionic/vue";
import { defineComponent } from "vue";
import { arrowBackOutline } from "ionicons/icons";

export default defineComponent({
  name: "WizardLayout",
  setup() {
    return {
      arrowBackOutline,
    };
  },
  data() {
    return {
      tituloHeader: "CREAR"
    }
  },
  components: {
    IonPage,
    IonHeader,
    IonToolbar,
    IonButtons,
    IonBackButton,
    IonTitle,
    IonContent,
    IonRouterOutlet,
  },
});
</script>

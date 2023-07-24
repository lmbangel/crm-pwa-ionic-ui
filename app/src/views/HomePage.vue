<template>
  <ion-header :translucent="true">
    <ion-toolbar>
      <!-- <ion-buttons slot="start">
        <ion-back-button default-href="#"></ion-back-button>
      </ion-buttons> -->
      <ion-title>{{ page }}</ion-title>
      <ion-buttons slot="end">
        <ion-button>
          <ion-icon slot="icon-only" :icon="search"></ion-icon>
        </ion-button>
      </ion-buttons>

      <ion-buttons slot="end">
        <ion-button>
          <ion-icon  slot="icon-only" :icon="notifications"></ion-icon>
        </ion-button>
      </ion-buttons>


      <ion-buttons slot="end">
        <ion-menu-button :auto-hide="false"></ion-menu-button>
      </ion-buttons>
    </ion-toolbar>
  </ion-header>
</template>

<script lang="ts">
import { IonBackButton, IonButton, IonButtons, IonIcon, IonMenuButton, IonTitle, IonToolbar, IonFooter, IonHeader } from '@ionic/vue';
import { create, ellipsisHorizontal, ellipsisVertical, helpCircle, search, personCircle, star, notifications} from 'ionicons/icons';
import { defineComponent } from 'vue';

export default defineComponent({
  components: {
    IonBackButton,
    IonButton,
    IonButtons,
    IonIcon,
    IonMenuButton,
    IonTitle,
    IonToolbar,
    IonFooter,
    IonHeader
  },
  setup() {
    return {
      create,
      ellipsisHorizontal,
      ellipsisVertical,
      helpCircle,
      search,
      personCircle,
      star
    };
  },
  data() {
    return {
      page: "Leads"
    }
  }
});
</script>

<style scoped></style>
<template>
  <ion-page
    class="ion-page">
    <ion-header>
      <ion-toolbar color="primary">
        <ion-buttons slot="start">
          <ion-back-button></ion-back-button>
        </ion-buttons>
        <ion-title>Home</ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content padding>
      <img alt="Vue logo" src="../assets/logo.png">
      <ion-button>Ionic</ion-button>
      <ion-button @click="openAbout()">About</ion-button>
    </ion-content>
  </ion-page>
</template>

<script>
// @ is an alias to /src
import { Component, Vue } from 'vue-property-decorator'
@Component({
  name: 'Home',
})
export default class Tabs extends Vue{
  openAbout() {
    this.$router.push('/about')
  }
}
</script>

<template>
  <v-app>
    <v-main>
      <HelloWorld />
    </v-main>
  </v-app>
</template>

<script setup>
// Import the functions you need from the SDKs you need
import { initializeApp } from "firebase/app";
// TODO: Add SDKs for Firebase products that you want to use
// https://firebase.google.com/docs/web/setup#available-libraries

// Your web app's Firebase configuration
const firebaseConfig = {
  apiKey: `${process.env.FIREBASE_API_KEY}`,
  authDomain: "t6-noodle.firebaseapp.com",
  databaseURL: "https://t6-noodle-default-rtdb.europe-west1.firebasedatabase.app",
  projectId: "t6-noodle",
  storageBucket: "t6-noodle.appspot.com",
  messagingSenderId: "1072421095024",
  appId: "1:1072421095024:web:7d5e319001d17d785ad6b5"
};

console.log(process.env.VUE_APP_FIREBASE_API_KEY); 
// Initialize Firebase
const app = initializeApp(firebaseConfig);
</script>

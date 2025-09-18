<script setup>
import { useRouter } from "vue-router";
import { defineProps } from "vue";

const props = defineProps(["event"]);
const router = useRouter()

const register = () => {
    router.push({
        name: 'EventDetails'
    })
}
</script>
<template>
  <p>Register for the event here</p>
  <button @click="register">Register Me!</button>
</template>

<template>
  <SignInButton />
  <SignOutButton v-if="isAuthenticated" />
</template>

<script setup lang="ts">
import SignInButton from './SignInButton.vue'
import SignOutButton from './SignOutButton.vue'
import { useIsAuthenticated } from '../composition-api/useIsAuthenticated'

const isAuthenticated = useIsAuthenticated()
</script>

<style scoped></style>

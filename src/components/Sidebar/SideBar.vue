<script setup>
import SkypeLogo from './SkypeLogo.vue';
import UserProfile from './UserProfile/UserProfile.vue'
import Conversations from './Conversations/Conversations.vue'
import MsLogo from './MsLogo.vue'
</script>
<template>
    <div class="sidebar">
        <SkypeLogo />
        <UserProfile />
        <Conversations />
        <MsLogo />
    </div>
</template>

<style>
.sidebar {
    border-right: 1px solid var(--border-color);
    display: grid;
    justify-items: center;
    grid-template-rows: 6.5rem 16rem 25.5rem auto;
}
</style>
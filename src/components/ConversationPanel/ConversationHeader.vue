<script setup>
import Profile from './Profile.vue'
import ConversationActions from './ConversationActions.vue';
</script>
<template>
    <div class="conversation-header">
        <Profile />
        <ConversationActions />
    </div>
</template>

<style>
.conversation-header {
    width: 55rem;
    height: 5rem;
    background-color: rgb(15, 15, 15, .5);
    border-radius: .8rem;
    margin-top: 1.7rem;
    padding: 0 1.5rem;
    display: flex;
    justify-content: space-between;
    align-items: center;
}
</style>
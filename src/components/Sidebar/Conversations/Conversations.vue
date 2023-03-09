<script setup>
import Conversation from './Conversation.vue'
</script>
<template>
    <div class="conversations">
        <h3>chats</h3>
        <Conversation v-for="n in 4"/>
    </div>
</template>

<style>
.conversations {
    width: 100%;
    display: grid;
    justify-items: center;
}

.conversations > h3 {
    width: 16rem;
    height: 2rem;
    text-transform: uppercase;
    border-bottom: .1rem solid rgba(255, 255, 255, .25);
    font-weight: 700;
    font-size: 1rem;
    line-height: 1.8rem;
    color: rgba(255, 255, 255, 0.25);
}
</style>
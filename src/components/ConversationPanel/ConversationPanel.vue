<script setup>
import ConversationHeader from './ConversationHeader.vue';
import MessageSection from './MessageSection.vue';
import ConversationInputSection from './ConversationInputSection.vue';
</script>
<template>
    <div class="conversation-panel">
        <ConversationHeader />
        <MessageSection />
        <ConversationInputSection />
    </div>
</template>

<style>
.conversation-panel {
    display: grid;
    justify-items: center;
    grid-template-rows: 6.8rem auto 5rem;
}
</style>
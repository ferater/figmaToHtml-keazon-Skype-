<script setup>
import ConversationDetail from './ConversationDetail.vue';
</script>
<template>
    <div class="conversation">
        <ConversationDetail />
    </div>
</template>

<style>
.conversation {
    width: 100%;
    height: 5.9rem;
    margin-top: .2rem;
    display: flex;
    justify-content: center;
    align-items: center;
}
.conversation:nth-child(3){
    background-color: #00B0F04D;
}
</style>
<script setup>
import Conversation from "./Conversation.vue";
import conversations from "./usersData";
</script>
<template>
  <div class="conversations">
    <h3>chats</h3>
    <Conversation v-for="n in conversations"  :message="n"/>
  </div>
</template>

<style>
.conversations {
  width: 100%;
  display: grid;
  justify-items: center;
grid-template-rows: 2.4rem auto;
}

.conversations > h3 {
  width: 16rem;
  height: 2rem;
  text-transform: uppercase;
  border-bottom: 0.1rem solid rgba(255, 255, 255, 0.25);
  font-weight: 700;
  font-size: 1rem;
  line-height: 1.8rem;
  color: rgba(255, 255, 255, 0.25);
}
</style>

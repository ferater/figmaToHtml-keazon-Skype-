<script setup>
import Conversation from "./Conversation.vue";
const conversations = [
  {
    pName: "Jessica White",
    pAvatar: "src/assets/img/jessica_white.jpg",
    pStatus: "online",
    mTime: "12:51 PM",
    message: "please help me! I fail reading",
    mStatus: "readed",
  },
  {
    pName: "Ryder Tiger",
    pAvatar: "src/assets/img/ryder_tiger.jpg",
    pStatus: "offline",
    mTime: "09:13 AM",
    message: "I'm a little sick, i may not join you",
    mStatus: "waiting",
  },
  {
    pName: "Agatha Stone",
    pAvatar: "src/assets/img/agatha_stone.jpg",
    pStatus: "offline",
    mTime: "02:02 AM",
    message: "Shall we go out in the morning",
    mStatus: "readed",
  },
  {
    pName: "Tomy Gily",
    pAvatar: "src/assets/img/tomy_gily.jpg",
    pStatus: "away",
    mTime: "11:41 PM",
    message: "New coffee has arrived An ",
    mStatus: "sent",
  }
];
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

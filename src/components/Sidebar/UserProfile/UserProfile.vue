<script setup>
import Avatar from '../../Avatar.vue';
import UserName from './UserName.vue';
import UserStatus from './UserStatus.vue';
const avatarProps = {
    imgPath: "src/assets/img/ugur_mercan.jpg",
    status:"online",
    width: "7.5rem",
    height: "7.5rem",
}
</script>
<template>
    <div class="user-profile">
        <Avatar v-bind="avatarProps" />
        <UserName />
        <UserStatus/>
    </div>
</template>

<style>
.user-profile {
    display: grid;
    justify-items: center;
    align-items: center;
    grid-template-rows: 8rem 2rem 1.5rem 3.3rem;
}
</style>
<script setup>
import Avatar from '../Avatar.vue';
const avatarProps = {
    imgPath: "src/assets/img/jessica_white.jpg",
    status:"online",
    width: "3.5rem",
    height: "3.5rem"
}
</script>
<template>
    <div class="profile">
        <Avatar v-bind="avatarProps" />
        <div class="profile-detail">
            <h3>Jessica White</h3>
            <span>Online</span>
        </div>
    </div>
</template>

<style>
.profile {
    width: 13rem;
    display: grid;
    grid-template-columns: auto auto;
    justify-items: space-evenly;
}

.profile .profile-detail{
    display: flex;
    flex-direction: column;
    justify-content: space-around;
}
.profile .profile-detail h3 {
    font-weight: 600;
    font-size: 1.1rem;
    line-height: 1.5rem;
    color: var(--hx-color);
}

.profile .profile-detail span {
    font-weight: 600;
    font-size: .8rem;
    line-height: 1.1rem;
    color: var(--span-color);
}
</style>
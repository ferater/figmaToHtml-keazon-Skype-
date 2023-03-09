<script setup>
import { Icon } from '@iconify/vue';
import Avatar from '../../Avatar.vue';
const avatarProps = {
    imgPath: "src/assets/img/agatha_stone.jpg",
    width: "3.5rem",
    height: "3.5rem",
}

</script>
<template>
    <div class="conversation-detail">
        <Avatar v-bind="avatarProps" />
        <div class="conversation-name">
            <h3>Jessica White</h3>
            <span>Please help me</span>
        </div>
        <div class="icon-tick">
            <Icon icon="mdi:tick-all" class="icon-edit x-scale" />
        </div>
        <div class="time">
            <span>12:51 PM</span>
        </div>
    </div>
</template>

<style>
.conversation-detail {
    width: 16rem;
    height: 3.5rem;
    position: relative;
    display: flex;
    justify-content: space-around;
}

.conversation-detail .time {
    font-weight: 400;
    font-size: .5rem;
    line-height: .7rem;
    color: rgba(255, 255, 255, 0.3);
    position: absolute;
    top: 0;
    right: 0;
}

.conversation-detail .conversation-name {
    display: flex;
    flex-direction: column;
    justify-content: space-around;
}

.conversation-detail .conversation-name h3 {
    font-weight: 700;
    font-size: 1.1rem;
    line-height: 1.5rem;
    color: #FFFFFF;
}

.conversation-detail .conversation-name span {
    font-weight: 400;
    font-size: .9rem;
    line-height: 1.1rem;
    color: rgba(255, 255, 255, 0.3);
}

.conversation-detail .icon-tick {
    height: 3.3rem;
    font-size: 1.2rem;
    color: #FFFFFF;
    display: grid;
    align-content: end;
}
</style>
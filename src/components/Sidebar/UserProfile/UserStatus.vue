<script setup>
import { Icon } from '@iconify/vue';
</script>
<template>
    <div class="user-status">
        <div class="user-emoticon">
            <Icon icon="noto:smiling-face-with-sunglasses" class="icon-emo" />
        </div>
        <span>I will be Skype developer</span>
        <Icon icon="ant-design:control-outlined" class="icon-settings x-scale c-pointer" />
    </div>
</template>

<style>
.user-status {
    width: 14rem;
    height: 2rem;
    border-radius: 2rem;
    background-color: rgba(15, 15, 15, .5);
    display: flex;
    justify-content: space-between;
    align-items: center;
    overflow: hidden;
    align-self: self-end;
}

.user-status .user-emoticon {
    width: 2.5rem;
    height: inherit;
    background-color: rgba(51, 51, 51, .5);
    display: grid;
    place-items: center;
}

.user-status span {
    font-weight: 400;
    font-size: .7rem;
    line-height: 1rem;
    color: rgba(255, 255, 255, 0.35);
}

.user-status .user-emoticon .icon-emo,
.user-status .icon-settings {
    font-size: 1.3rem;
}

.user-status .icon-settings {
    color: rgba(139, 138, 138, 0.5);
    margin-right: .75rem;
}</style>
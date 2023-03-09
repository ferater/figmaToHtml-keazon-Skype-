<script setup>
import { Icon } from '@iconify/vue';
</script>
<template>
    <div class="conversation-input-section">
        <div class="input-icon">
            <Icon icon="mdi:plus" class="icon-plus x-scale c-pointer" />
        </div>
        <div class="conversation-input">
            <input type="text" placeholder="Type a message..." name="chat" class="chat" />
            <Icon icon="mdi:attach-file" class="icon-attach x-scale c-pointer" />
        </div>
        <div class="input-icon">
            <Icon icon="ic:outline-emoji-emotions" class="icon-drive x-scale c-pointer" />
        </div>
        <div class="input-icon">
            <Icon icon="basil:google-drive-outline" class="icon-emo x-scale c-pointer" />
        </div>
    </div>
</template>

<style>
.conversation-input-section {
    width: 55rem;
    height: 3.5rem;
    display: grid;
    grid-template-columns: 3.5rem 40rem 3.5rem 3.5rem;
    justify-content: space-between;
}

.conversation-input-section .input-icon {
    width: 3.5rem;
    height: 3.5rem;
    border-radius: 50%;
    background-color: rgba(0, 176, 240, .1);
    box-shadow: 0px 4px 30px rgba(0, 0, 0, 0.5);
    display: grid;
    place-items: center;
}

.conversation-input-section .input-icon .icon-plus,
.conversation-input-section .input-icon .icon-emo,
.conversation-input-section .input-icon .icon-drive {
    font-size: 2rem;
    color: #00B0F0;
}

.conversation-input-section div.conversation-input input[name='chat'] {
    width: 100%;
    height: 3.5rem;
    padding: 0 1.5rem;
    outline: none;
    border: 1px solid #00B0F0;
    border-radius: 1.2rem;
    background-color: rgba(15, 15, 15, .3);

}

.conversation-input-section div.conversation-input input[name='chat']::placeholder,
.conversation-input-section div.conversation-input input[name='chat'] {
    font-weight: 600;
    font-size: 1.1rem;
    line-height: 1.5rem;
    color: rgba(255, 255, 255, 0.2);
}

.conversation-input-section div.conversation-input {
    position: relative;
}

.conversation-input-section div.conversation-input .icon-attach {
    font-size: 1.9rem;
    color: rgba(255, 255, 255, .3);
    position: absolute;
    right: 1rem;
    top:50%;
    translate: 0 -50%;
}
</style>
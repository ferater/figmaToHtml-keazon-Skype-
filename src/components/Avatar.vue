<script setup>
import Badge from './Badge.vue';
const props = defineProps({
    imgPath: String,
    status: String,
    width: String,
    height: String
});
</script>
<template>
    <div class="avatar-container">
        <img :src="imgPath" alt="" class="avatar">
        <!-- this badge prop is user status -->
        <Badge :status="status" />
    </div>
</template>
<style>
.avatar-container {
    width: v-bind('width');
    height: v-bind('height');
    background-color: var(--border-color);
    border: .1rem solid var(--border-color);
    border-radius: 50%;
    display: flex;
    justify-content: center;
    align-items: center;
    position: relative;
}

.avatar-container img.avatar {
    width: v-bind('width');
    height: v-bind('height');
    border-radius: inherit;
    border: .1rem solid var(--border-color);
    object-fit: cover;
}
</style>
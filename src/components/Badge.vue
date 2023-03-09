<script setup>
defineProps({
    status:String,
})
</script>
<template>
    <div class="badge" :class="status"></div>
</template>

<style>
.badge{
    width: 1rem;
    height: 1rem;
    border-radius: 50%;
    position: absolute;
    bottom: 0;
    right: -.3rem;
}
.online{
    background-color: var(--online-color);
}
.offline{
    background-color: var(--offline-color);
}
</style>
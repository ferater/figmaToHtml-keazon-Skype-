<script setup>
defineProps({
    status: String,
})
</script>
<template>
    <div class="badge" :class="status"></div>
</template>

<style>
.badge::after,
.badge {
    position: absolute;
    border-radius: 50%;

}

.badge {
    width: 1rem;
    height: 1rem;
    bottom: 0;
    right: -.3rem;
}

.badge::after {
    content: '';
    inset: -.4rem;
    background-color: rgba(0, 0, 0, .5);
    z-index: -1;

}

.online {
    background-color: var(--online-color);
}

.offline {
    background-color: var(--offline-color);
}
.away {
    background-color: var(--away-color);
}
</style>
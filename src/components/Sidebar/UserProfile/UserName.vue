<script setup>
import { Icon } from '@iconify/vue';
</script>
<template>
    <div class="user-name">
        <h3>Uğur MERCAN</h3>
        <Icon icon="majesticons:edit-pen-2-line" class="icon-edit x-scale c-pointer" />
    </div>
    <div class="nick-name">
        <h5>@keazon</h5>
    </div>
</template>
<style>
.user-name {
    display: flex;
    align-items: center;
}

.user-name h3,
.user-name .icon-edit {
    font-size: 1.2rem;
    font-weight: 600;
    line-height: 2rem;
}

.user-name h3 {
    color: rgba(255, 255, 255, 0.7);
}

.user-name .icon-edit {
    color: var(--border-color);
    margin-left: .5rem;
}

.nick-name h5 {
    font-weight: 400;
    font-size: 1rem;
    line-height: 1.4rem;
    color: rgba(255, 255, 255, .3);
}
</style>
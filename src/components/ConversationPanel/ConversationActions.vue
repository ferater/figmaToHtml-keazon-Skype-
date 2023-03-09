<script setup>
import { Icon } from '@iconify/vue';
</script>
<template>
    <div class="conversation-actions">
        <div class="action-icon">
            <Icon icon="la:phone-solid" class="icon-action x-scale c-pointer" />
        </div>
        <div class="action-icon">
            <Icon icon="iconoir:facetime" class="icon-action x-scale c-pointer" />
        </div>
        <div class="action-icon">
            <Icon icon="material-symbols:settings-outline" class="icon-action x-scale c-pointer" />
        </div>
    </div>
</template>

<style>
.conversation-actions {
    width: 11rem;
    height: 2.5rem;
    display: flex;
    justify-content: space-between;
}

.conversation-actions .action-icon {
    width: 2.5rem;
    height: 2.5rem;
    border-radius: 50%;
    background: rgba(0, 176, 240, 0.1);
    box-shadow: 0px 4px 50px rgba(0, 0, 0, 0.15);
    display: grid;
    place-items: center;
}

.conversation-actions .icon-action {
    font-size: 1.5rem;
    color: rgba(255, 255, 255, 0.695);
}
</style>
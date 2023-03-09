<script setup>
import { computed } from 'vue';
import { Icon } from '@iconify/vue';
import Avatar from '../../Avatar.vue';
const props = defineProps({
    pName: String,
    pAvatar: String,
    pStatus: String,
    mTime: String,
    message: String,
    mStatus: String,
});
const avatarProps = {
    imgPath: props.pAvatar,
    status:props.pStatus,
    width: "3.5rem",
    height: "3.5rem",
};
const tickIcon = computed(()=> {
    if(props.mStatus != 'waiting') {
        return 'mdi:tick-all'
    }else {
        return 'mdi:tick'
    }
});
</script>
<template>
    <div class="conversation-detail">
        <Avatar v-bind="avatarProps" />
        <div class="conversation-name">
            <h3>{{ pName }}</h3>
            <h5 class="message">{{ message }}</h5>
        </div>
        <div class="tick-icon">
            <Icon :icon="tickIcon" class="icon-tick x-scale" :class="mStatus" />
        </div>
        <div class="time">
            <span>{{ mTime }}</span>
        </div>
    </div>
</template>

<style>
.conversation-detail {
    width: 16rem;
    height: 3.5rem;
    position: relative;
    display: flex;
    justify-content: space-between;
}

.conversation-detail .time {
    font-weight: 400;
    font-size: .5rem;
    line-height: .7rem;
    color: var(--span-color);
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
    color: var(--hx-color);
}

.conversation-detail .conversation-name h5.message {
    font-weight: 400;
    font-size: .9rem;
    line-height: 1.1rem;
    color: var(--span-color);
    width: 9rem;
    overflow: hidden;
    white-space: nowrap;
    text-overflow: ellipsis;
   
}

.conversation-detail div.tick-icon {
    height: 3.3rem;
    font-size: 1.2rem;
    color: var(--hx-color);
    display: grid;
    align-content: end;
}
.conversation-detail div.tick-icon .icon-tick.readed {
    color: #00B0F0;
}
</style>
<template>
    <div class="message-section">
        <div class="message from single">
            <span>Hi, Ugur </span>
        </div>
        <div class="message me single">
            <span>Hi, Jessica! </span>
        </div>
    </div>
</template>

<style>
.message-section {
    width: 55rem;
    padding: 3rem;
    display: flex;
    justify-content: space-between;
    background-color: #fff;
}

.message-section .message {
    position: relative;
}

.message-section .message.me,
.message-section .message.from {
    width: fit-content;
    height: fit-content;
    padding: .7rem 1.5rem;
    border-radius: 1rem;
}

.message-section .message.from {
    background-color: #282828;
}

.message-section .message.me {
    background-color: #00B0F0;
}

.message-section .message.from span,
.message-section .message.me span {
    font-weight: 400;
    font-size: 1.1rem;
    line-height: 1.5rem;
    color: #FFFFFF;
}

.message-section .message.from.single::after {
    content: '';
    position: absolute;
    bottom: -7px;
    left: 20%;
    border-bottom: 10px solid #282828;
    border-right: 10px solid #282828;
    border-left: 5px solid transparent;
    border-top: 5px solid transparent;
    rotate: 45deg;
}
</style>
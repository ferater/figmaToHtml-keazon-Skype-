<template>
    <div class="message-section">
        <div class="message from single">
            <span>Hi, Ugur </span>
        </div>
        <div class="message me single">
            <span>Hi, Jessica! </span>
        </div>
        <div class="message from">
            <span>We are watching movie in Netflix right now! </span>
        </div>
        <div class="message from">
            <img src="../../assets/img/sp_active.png" alt="">
        </div>
        <div class="message from single">
            <span>We are waiting for you</span>
        </div>
        <div class="message me single">
            <span>Please help me! I fail to reach Netflix... I guess my Netflix crash. Are you wanna listening to
                music?</span>
        </div>
    </div>
</template>

<style>
.message-section {
    width: 55rem;
    padding: 3rem;
    display: flex;
    flex-direction: column;
}

.message-section .message {
    position: relative;
    transition: all .2s ease;
}

.message-section .message img {
    max-width: 100%;
}

.message-section .message.me,
.message-section .message.from {
    width: fit-content;
    max-width: 60%;
    height: fit-content;
    padding: .7rem 1.5rem;
    border-radius: 1rem;
    margin-top: .4rem;
}

.message-section .message.from {
    background-color: var(--message-from);
}

.message-section .message.me {
    align-self: flex-end;
    background-color: var(--message-me);
}


.message-section .message.from span,
.message-section .message.me span {
    font-weight: 400;
    font-size: 1.1rem;
    line-height: 1.5rem;
    color: var(--hx-color);
}

.message-section .message.me.single::after,
.message-section .message.from.single::after {
    content: '';
    position: absolute;
    bottom: -7px;
    border-left: 5px solid transparent;
    border-top: 5px solid transparent;
    rotate: 45deg;
}

.message-section .message.from.single::after {
    border-bottom: 10px solid var(--message-from);
    border-right: 10px solid var(--message-from);
    left: 20%;

}

.message-section .message.me.single::after {
    border-bottom: 10px solid var(--message-me);
    border-right: 10px solid var(--message-me);
    right: 20%;
}
</style>
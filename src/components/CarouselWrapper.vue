<template>
    <div class="carousel">
        <ul class="carousel-viewport">
            <slot />
        </ul>
    </div>
</template>

<style scoped>
    .carousel {
        width: 100%;
        height: 100%;
        position: relative;
    }

    .carousel::before {
        content: '\276E';
        font-weight: bolder;
        color: #fff;
        position: absolute;
        top: 50%;
        left: 0;
        width: 10%;
        transform: translateY(-50%);
        text-align: center;
        font-size: 32px;
    }

    .carousel::after {
        content: '\276F';
        font-weight: bolder;
        color: #fff;
        position: absolute;
        top: 50%;
        right: 0;
        width: 10%;
        transform: translateY(-50%);
        text-align: center;
        font-size: 32px;
    }

    .carousel-viewport {
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        list-style: none;
        margin: 0;
        padding: 0;
        display: flex;
        overflow-x: scroll;
        overflow-y: hidden;
        scroll-behavior: smooth;
        scroll-snap-type: x mandatory;
        scrollbar-width: 0;
        -ms-overflow-style: 0;
    }

    .carousel-viewport::-webkit-scrollbar {
        display: none;
    }
</style>
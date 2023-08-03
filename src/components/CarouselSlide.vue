<script setup>
defineProps({
    name: {
        type: String,
        required: true
    },
    prev: {
        type: String,
        required: true
    },
    next: {
        type: String,
        required: true
    }
})
</script>

<template>
    <li :id="name" class="carousel-slide">
        <a :href="`#${prev}`" class="carousel-prev"></a>
        <div class="carousel-content">
            <slot />
        </div>
        <a :href="`#${next}`" class="carousel-next"></a>
    </li>
</template>

<style scoped>
.carousel-slide {
    list-style: none;
    margin: 0;
    padding: 0;
    position: relative;
    flex: 0 0 100%;
    width: 100%;
    display: flex;
    justify-content: space-between;
    scroll-snap-align: center;
}

.carousel-prev,
.carousel-next {
    z-index: 1;
    width: 10%;
    height: 100%;
}

.carousel-content {
    width: 80%;
    height: 100%;
    border-radius: 24px;
    overflow: hidden;
}
</style>

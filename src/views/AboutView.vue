<script setup>
import PageTitle from "@/components/PageTitle.vue"
</script>

<template>
    <PageTitle title="About" />

    <div class="content">
        Sexpression:&#8203;Newcastle is a thing
    </div>
</template>

<style scoped>
@import "@/assets/view.css";

.content {
    width: 90%;
    display: flex;
    font-size: min(6vw, 4vh);
    color: #fff;
    border-radius: 24px;
    overflow: hidden;
    background: #1a60d688;
    padding: 2vh;
}

</style>

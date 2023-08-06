<script setup>
import PageTitle from "@/components/PageTitle.vue"
</script>

<template>
    <PageTitle title="About" />

    <div class="content">
        <div class="img">
            <img src="@/assets/img/logo_full_nobg.png" alt="sexpression newcastle logo" />
        </div>
        <hr />
        <div class="info">Sexpression:&#8203;Newcastle is a thing</div>
    </div>
</template>

<style scoped>
@import "@/assets/view.css";

.content {
    width: 90%;
    display: flex;
    border-radius: 24px;
    overflow: hidden;
    background: #00000020;
}

.content hr {
    border: 1px solid #00000020;
}

.content .img {
    height: 100%;
    aspect-ratio: 1 / 1;
    position: relative;
}

.img img {
    position: absolute;
    top: 0;
    left: 0;
    height: 100%;
}
</style>

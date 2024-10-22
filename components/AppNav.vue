<template>
    <nav class="nav">
        <ul class="nav__list">
            <li class="nav__item">탭 이름</li>
            <li class="nav__item">탭 이름</li>
            <li class="nav__item">탭 이름</li>
            <li class="nav__item">탭 이름</li>
            <li class="nav__item">탭 이름</li>
        </ul>
    </nav>
</template>

<script setup lang="ts">
const navItems = reactive([
    {
        id: 1,
        label: "일반시사",
        value: "General",
    },
    {
        id: 2,
        label: "비즈니스",
        value: "Business",
    },
    {
        id: 3,
        label: "엔터테인먼트",
        value: "Entertainment",
    },
    {
        id: 4,
        label: "",
        value: "General",
    },
    {
        id: 5,
        label: "일반시사",
        value: "General",
    },
    {
        id: 6,
        label: "일반시사",
        value: "General",
    },
]);
</script>

<style lang="scss" scoped>
.nav {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 100%;
    margin-top: 100px;

    &__list {
        display: flex;
        justify-content: center;
        align-items: center;
        list-style-type: none;
        width: 100%;
        gap: 24px;
    }

    &__item {
        display: flex;
        justify-content: center;
        align-items: center;
        padding: 6px 12px;
        background-color: $color-gray-200;
        border-radius: 20px;
        color: $color-black-700;
        cursor: pointer;
    }
}
</style>

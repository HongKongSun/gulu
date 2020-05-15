<template>
<!-- 放html -->
    <button class="g-button">按钮</button>
</template>

<script>
export default {
    // 放 js 代码
    // 不需要Vue.conponent
    
}
</script>

<style lang="scss" scoped>
    .g-button {
        font-size: var(--font-size);
        height: var(--button-height);
        padding: 0 1em;
        border-radius: var(--border-radius);
        border: 1px solid var(--border-color);
        background: var(--button-bg);
        .g-button:hover {
        border-color: var(--border-color-hover);
    }
    // 套用 而且不需要重复 写当前选择器，而是用 & 代替
    &:active {
        background-color: var(--button-active-bg);
    }
    &:focus {
        outline: none;
    }
    }
    
</style>
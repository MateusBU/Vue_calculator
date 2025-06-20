<template>
    <div class="calculator">
        <appButton />
        <appDisplay />
    </div>
</template>

<script>
import appDisplay from '@/components/compDisplay.vue';
import appButton from '@/components/compButton.vue';

export default{
    components: {appButton, appDisplay}
}
</script>

<style>
.calculator{
    height: 320px;
    width: 235px;
    border-radius: 5px;
    overflow: hidden;

    display: grid;
    grid-template-columns: repeat(4, 25%);
    grid-template-rows: 1fr 48px 48px 48px 48px 48px;
}
</style>

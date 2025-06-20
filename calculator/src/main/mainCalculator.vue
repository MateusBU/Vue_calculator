<template>
    <div class="calculator">
        <appDisplay />
        <appButton label="AC" triple/>
        <appButton label="/" operation/>
        <appButton label="7"/>
        <appButton label="8"/>
        <appButton label="9"/>
        <appButton label="*" operation/>
        <appButton label="4"/>
        <appButton label="5"/>
        <appButton label="6"/>
        <appButton label="-" operation/>
        <appButton label="1"/>
        <appButton label="2"/>
        <appButton label="3"/>
        <appButton label="+" operation/>
        <appButton label="0" fouble/>
        <appButton label="."/>
        <appButton label="=" operation/>
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

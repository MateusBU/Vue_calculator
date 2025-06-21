<template>
    <div class="calculator">
        <appDisplay value="100"/>
        <appButton label="AC" triple @onCalcButtonClick="clearMemory"/>
        <appButton label="/" operation @onCalcButtonClick="setOperation"/>
        <appButton label="7" @onCalcButtonClick="addDigit"/>
        <appButton label="8" @onCalcButtonClick="addDigit"/>
        <appButton label="9" @onCalcButtonClick="addDigit"/>
        <appButton label="*" operation @onCalcButtonClick="setOperation"/>
        <appButton label="4" @onCalcButtonClick="addDigit"/>
        <appButton label="5" @onCalcButtonClick="addDigit"/>
        <appButton label="6" @onCalcButtonClick="addDigit"/>
        <appButton label="-" operation @onCalcButtonClick="setOperation"/>
        <appButton label="1" @onCalcButtonClick="addDigit"/>
        <appButton label="2" @onCalcButtonClick="addDigit"/>
        <appButton label="3" @onCalcButtonClick="addDigit"/>
        <appButton label="+" operation @onCalcButtonClick="setOperation"/>
        <appButton label="0" double @onCalcButtonClick="addDigit"/>
        <appButton label="." @onCalcButtonClick="addDigit"/>
        <appButton label="=" operation @onCalcButtonClick="setOperation"/>
    </div>
</template>

<script>
import appDisplay from '@/components/compDisplay.vue';
import appButton from '@/components/compButton.vue';

export default{
    components: {appButton, appDisplay},
    methods:{
        clearMemory(){
            
        },
        setOperation(operation){
            
        },
        addDigit(n){

        }
    }
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

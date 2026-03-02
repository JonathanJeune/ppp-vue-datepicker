<template>
    <div class="wrapper">
        <VueDatePicker 
            v-model="selectedDate" 
            placeholder="Select Date" 
            :auto-apply="true" 
            :config=" { keepActionRow: true }"
            :action-row="{ showSelect: false, showCancel: false, showNow: true, showClear: true, showPreview: false }" 
            clear-button-label="Tout effacer" 
        />
    </div>
</template>

<script lang="ts" setup>
    import { ref } from 'vue';
    import { VueDatePicker } from '../src';

    const selectedDate = ref();
</script>

<style lang="scss">
    .wrapper {
        padding: 200px;
    }
</style>

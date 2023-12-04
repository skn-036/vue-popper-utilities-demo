<script setup>
import DropdownWithChildren from './components/DropdownWithChildren.vue';
import Tooltip from './components/Tooltip.vue';
import CustomDropdown from './components/CustomDropdown.vue';
import FocusTrigger from './components/FocusTrigger.vue';
</script>

<template>
    <div class="w-full flex flex-col gap-24 p-4">
        <DropdownWithChildren />

        <CustomDropdown />

        <Tooltip />

        <FocusTrigger />
    </div>
</template>

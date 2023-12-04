<script setup>
import { Tooltip } from 'vue-popper-utilities';
</script>

<template>
    <div class="w-full flex flex-col gap-4">
        <div class="font-bold text-black text-xl underline">Tooltip</div>

        <div class="w-max">
            <Tooltip
                placement="bottom-start"
                text="Lorem ipsum dolor sit amet consectetur adipisicing elit. Quaerat aut repellat magnam deleniti porro veniam ipsam molestias odit nostrum minima quis, quas, mollitia fugiat atque, possimus nihil ratione debitis unde."
            >
                <template #reference>
                    <button
                        class="px-4 py-2 rounded bg-rose-600 text-white flex flex-start justify-between gap-4"
                    >
                        <div>Tooltip button</div>
                    </button>
                </template>
            </Tooltip>
        </div>
    </div>
</template>

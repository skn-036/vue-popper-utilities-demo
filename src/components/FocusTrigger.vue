<script setup>
import { Tooltip } from 'vue-popper-utilities';
</script>

<template>
    <div class="w-full flex flex-col gap-4">
        <div class="font-bold text-black text-xl underline">
            Trigger on focus
        </div>

        <div class="w-max">
            <Tooltip
                trigger="focus"
                placement="bottom-start"
                text="Lorem ipsum dolor sit amet consectetur adipisicing elit. Quaerat aut repellat magnam deleniti porro veniam ipsam molestias odit nostrum minima quis, quas, mollitia fugiat atque, possimus nihil ratione debitis unde."
            >
                <template #reference>
                    <input
                        class="w-full p-2 rounded outline-none ring-2 ring-gray-400 focus:ring-rose-500"
                        placeholder="trigger on focus"
                    />
                </template>
            </Tooltip>
        </div>
    </div>
</template>

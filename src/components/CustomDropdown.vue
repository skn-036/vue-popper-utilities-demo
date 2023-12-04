<script setup>
import { Popup } from 'vue-popper-utilities';
</script>

<template>
    <div class="w-full flex flex-col gap-4">
        <div class="font-bold text-black text-xl underline">Custom popup</div>

        <div class="w-max">
            <Popup>
                <template #reference="{ isOpen }">
                    <button
                        class="px-4 py-2 rounded bg-rose-600 text-white flex flex-start justify-between gap-4"
                    >
                        <div>Custom popup</div>
                        <div
                            class="transition duration-300"
                            :class="[isOpen ? 'rotate-180' : '']"
                        >
                            &#x25BC;
                        </div>
                    </button>
                </template>

                <div
                    class="p-4 w-[320px] flex flex-col gap-4 bg-white rounded border border-gary-300 shadow-md shadow-rose-300"
                >
                    <div class="flex flex-col gap-1">
                        <label class="font-bold">Email</label>
                        <input
                            class="w-full p-2 rounded outline-none ring-2 ring-gray-400 focus:ring-rose-500"
                        />
                    </div>

                    <div class="flex flex-col gap-1">
                        <label class="font-bold">Password</label>
                        <input
                            class="w-full p-2 rounded outline-none ring-2 ring-gray-400 focus:ring-rose-500"
                        />
                    </div>

                    <button class="w-full bg-rose-500 text-white rounded py-2">
                        Submit
                    </button>
                </div>
            </Popup>
        </div>
    </div>
</template>

<template>
    <div>
        <br>
        <div class="w-1/2 p-4 mx-auto text-center border">
            <br>
            <div
                class="w-full max-w-sm bg-white border border-gray-200 rounded-lg shadow dark:bg-gray-800 dark:border-gray-700">
                <div class="flex flex-col items-center pb-10">
                    <h5 class="mb-1 text-xl font-medium text-gray-900 dark:text-white">{{ user.user_metadata.full_name
                        }}</h5>
                    <span class="text-sm text-gray-500 dark:text-gray-400">Email: {{ user.user_metadata.email }}</span>
                    <span class="text-sm text-gray-500 dark:text-gray-400">ID: {{ user.id }}</span>
                </div>
            </div>
            <br>
        </div>

    </div>
</template>

<script setup>
const user = useSupabaseUser()

</script>
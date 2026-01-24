<template>
    <div class="mt-10 grid grid-cols-[80%_20%]">
        <div class="text-4xl">
            <div v-html="text"></div>
            <hr class="mt-2">
        </div>
        <div class="m-1 row-span-2 rounded-md py-[3em] px-[1em] bg-blue-700 font-bold text-2xl text-white text-center ">
            {{ btn }}
        </div>
        <div class="flex text-gray text-lg">
            <div class="mr-10">
                <p class="text-xs font-bold">Email:</p>
                {{ email }}
            </div>
            <div>
                <p class="text-xs font-bold">Phone:</p>
                {{ phone }}
            </div>
        </div>
        <form action="" method="post">
            <input type="text" name="subject" id="">
            <input type="text" name="content" id="">
            <input type="submit" value="">
        </form>
    </div>
</template>
<script setup lang="ts">
interface Props {
    text:string;
    btn:string;
    email:string;
    phone:string;
}

defineProps<Props>();
</script>
<template>
    <section class="flex justify-between">
        <div>
            「雨が降っても　花は咲くから　前を向いて」<br />
            "Even if it rains, flowers will still bloom, so keep looking
            forward."<br />
            <p>-"lilac" by Mrs. Green Apple</p>
        </div>
        <div class="text-1xl max-w-3xs text-gray-500">
            <p>
                Lorem ipsum dolor, sit amet consectetur adipisicing elit. Lorem
                ipsum dolor, sit amet consectetur adipisicing elit.
            </p>
            <p class="text-black-800 bold text-3xl mt-2">More about me!</p>
        </div>
    </section>
</template>
<script setup lang="ts">
    interface Props{
        text:string;
        translation:string;
        source:string;
    }
    defineProps();
</script>
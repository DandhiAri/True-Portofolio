<template>
    <div class="bg-neutral-900 text-xl p-5 grid content-center text-white text-center h-15">
        <p class="flex justify-center"> 
            <div class="cursor-pointer underline mr-1" @click="copyURL"> Email: dandhiari (at) gmail [dot] com </div> | 
            <div v-show="phone"> Phone: {{phone}} } | </div> 
            <a class="underline ml-1" href="{{ github }}">Github: @DandhiAri</a>
        </p>
    </div>
</template>
<script setup >
const props = defineProps({
    email: String,
    // phone: String,
    github: String
});
const copyURL = () => {
    navigator.clipboard.writeText(props.email)
        .then(() => {
            alert('Email address copied to clipboard!');
        })
        .catch(err => {
            console.error('Failed to copy email address: ', err);
        });
};
</script>

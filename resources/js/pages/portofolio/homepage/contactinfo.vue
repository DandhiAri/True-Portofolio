<template>
    <div class=" bg-neutral-900 text-md p-2 grid content-center text-white text-center">
        <div class="flex justify-center">
            <div @mouseenter="activeMouse = 'email'" @mouseleave="activeMouse = ''"
                :class="activeMouse === 'email' ? 'underline decoration-1 underline-offset-4' : ''" 
                class="cursor-pointer mr-1 transition-all" 
                @click="copyURL">
                Email: dandhiari (at) gmail [dot] com
            </div>
            |
            <a @mouseenter="activeMouse = 'github'" @mouseleave="activeMouse = ''"
                :class="{ 'underline': activeMouse === 'github' }" class="ml-1" :href="props.github" target="_blank">
                Github: (at) DandhiAri
            </a>
        </div>
    </div>
</template>
<script setup>
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

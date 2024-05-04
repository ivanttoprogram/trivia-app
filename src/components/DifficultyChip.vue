<script setup>
const props = defineProps({
    difficulty: {
        type: String, 
        required: true, 
    }
})
</script>

<template>
    <P class="px-4 py-2 rounded-full border absolute uppercase text-white bottom-5 left-8 text-2xl font-bold"
    :class="props.difficulty === 'easy' ? 'bg-green-800' : props.difficulty === 'medium' ? 'bg-yellow-700' : 'bg-red-800' ">
    {{ props.difficulty }}
    </P>
</template>
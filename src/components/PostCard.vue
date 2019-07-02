<template>
    <div class="border-2 p-4 mb-4 w-full cursor-pointer hover:bg-gray-200">
        <h2 class="font-semibold text-xl">{{ post.title }}</h2>
    </div>
</template>

<script>
export default {
    props: ['post']
}
</script>

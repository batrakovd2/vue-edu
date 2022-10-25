<template>
    <div>
        <div>Like: {{ likes }}</div>
        <div>Dislike: {{ dislikes }}</div>
        <button>Кнопка like</button>
        <button>Кнопка dislike</button>
    </div>
</template>

<script>
    export default {
        data() {
            return {
                likes: 0,
                dislikes: 5,
            }
        }
    }
</script>

<style>

</style>


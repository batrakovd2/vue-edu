<template>
    <div>
        <form @submit.prevent>
            <h4>Создание поста</h4>
            <input v-bind:value="title" @input="title = $event.target.value" class="input-control" type="text" placeholder="Название" />
            <input v-bind:value="body" @input="body = $event.target.value" class="input-control" type="text" placeholder="Описание" />
            <button class="btn" @click="createPost">Создать</button>
        </form>
    </div>
</template>

<script>
export default {

}
</script>

<style>

</style>
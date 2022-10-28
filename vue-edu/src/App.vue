<template>
    <div class="app">
        <form>
            <h4>Создание поста</h4>
            <input class="input-control" type="text" placeholder="Название" />
            <input class="input-control" type="text" placeholder="Описание" />
            <button class="btn">Создать</button>
        </form>
        <div class="post" v-for="post in posts">
            <strong>{{ post.title }}</strong>
            <p>{{ post.body }}</p>    
        </div>
    </div>
</template>

<script>
    export default {
        data() {
            return {
                posts: [
                    {id: 1, title: 'title 1', body: 'body 1'},
                    {id: 2, title: 'title 2', body: 'body 2'},
                    {id: 3, title: 'title 3', body: 'body 3'}
                ]
            }
        },
        methods: {

        }
    }
</script>

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

.app{
    padding: 20px;
}

.post{
    padding: 15px;
    border: 2px solid teal;
    margin: 15px 20px;
}

form{
    display: flex;
    flex-direction: column;
}

.input-control{
    width: 100%;
    border: 1px solid teal;
    padding: 10px 15px;
    margin-top: 15px;
}

.btn{
    margin-top: 15px;
    align-self: end;
    padding: 10px 15px;
    background: none;
    border: 1px solid teal;
    color: teal;
}
</style>


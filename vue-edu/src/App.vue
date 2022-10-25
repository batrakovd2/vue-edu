<template>
    <div>
        <div class="post">
            <strong>Название </strong>
            <p>Пост о JS</p>    
        </div>
        <div class="post">
            <strong>Название </strong>
            <p>Пост о JS</p>    
        </div>
        <div class="post">
            <strong>Название </strong>
            <p>Пост о JS</p>    
        </div>
    </div>
</template>

<script>
    export default {
        data() {
            return {
                likes: 0,
                dislikes: 5,
            }
        },
        methods: {
            addLike() {
                this.likes += 1;
            },
            addDislike() {
                this.dislikes += 1;
            }
        }
    }
</script>

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

.post{
    padding: 15px;
    border: 2px solid teal;
    margin: 15px 20px;
}
</style>


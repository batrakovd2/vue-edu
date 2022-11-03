<template>
    <div class="app">

        
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
                ],
                title: '',
                body: ''
            }
        },
        methods: {
            createPost() {
                const newPost = {
                    id: Date.now(),
                    title: this.title,
                    body: this.body
                }
                this.posts.push(newPost)
                this.title = ''
                this.body = ''
            },
            // inputTitle(event) {
            //     console.log(event)
            // }
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


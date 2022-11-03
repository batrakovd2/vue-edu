<template>
    <div>
        <div class="post" v-for="post in posts">
            <strong>{{ post.title }}</strong>
            <p>{{ post.body }}</p>    
        </div>
    </div>
</template>

<script>
export default {

}
</script>

<style>
.post{
    padding: 15px;
    border: 2px solid teal;
    margin: 15px 20px;
}
</style>
<template>
    <Layout>
        <div v-html="$page.post.content"/>
    </Layout>
</template>

<page-query>
query Post ($path: String!){
    post: post (path: $path) {
        title
        content
    }
}
</page-query>

<script>
export default {
    metaInfo() {
        return {
            title: this.$page.post.title
        }
    }
}
</script>
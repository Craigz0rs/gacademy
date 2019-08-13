<template>
    <Layout>

    </Layout>
</template>
<page-query>
query Post ($path: String!) {
    wordPressPost (path: $path) {
        title
    }
}
</page-query>
<script>
export default {
    
}
</script>
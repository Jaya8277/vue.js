<template>
<h1>HTML binding</h1>
<h1>{{text}}</h1>
<!-- {{ tag }} -->
<div v-html="tag"></div>
<div v-html="tag2"></div>
</template>

<script>
export default {
    name: 'HtmlBinding',
    data() {
        return {
            text: "Jaya",
            tag: "<h1>Vishwakarma</h1>",
            tag2: "<h1>jaya@gmail.com</h1>"
        }
    }
}
</script>

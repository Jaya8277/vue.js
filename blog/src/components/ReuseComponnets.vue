<template>
<h1>Reuse Components</h1>
<ul>
    <li v-for="item in users" :key="item.name">
        <User :data="item" :getData="getData"/>
        <!-- {{ item.name }}

        {{ item.email }} -->

    </li>
</ul>

</template>

<script>
import User from './User.vue'
export default {
    name: 'ReuseComponnets',
    components: {
        User
    },
    methods:{
        getData(name){
            alert(name)
        }

    },
    data() {
        return {
            users: [{
                    name: 'jaya',
                    email: 'jaya@gmail.com'
                },
                {
                    name: 'Rohit',
                    email: 'rohit@gmail.com'
                },
                {
                    name: 'Rema',
                    email: 'rema@gmail.com'
                },
                {
                    name: 'Arjun',
                    email: 'arjun@gmail.com'
                },
                {
                    name: 'Risi',
                    email: 'risi@gmail.com'
                }
            ]
        }
    }
}
</script>

<style scoped>
h1 {
    color: orange
}
</style>

<template>
<h1>For Loop in vue js</h1>
<ul>
    <li v-for="item in technology" :key="item">
        {{ item }}
    </li>
</ul>
<br/><br/>
<ul>
    <li v-for="item in users" :key="item.email">
Name is :{{item.name}} and Email is :{{item.email}}
    </li>
</ul>
</template>

<script>
export default {
    name: 'ForLoop',
    data() {
        return {
            technology: ["java", "php", "html", "node"],
            users:[
               {
                name:"Jaya",
                email:"jaya@gmail.com"
               },
               {
                name:"Arav",
                email:"Arav@gmail.com"
               },
               {
                name:"Shanvi",
                email:"Shanvi@gmail.com"
               },
               {
                name:"Anu",
                email:"Anu@gmail.com"
               },
               {
                name:"Aarushi",
                email:"Aarushi@gmail.com"
               }
            ]
        }
    }
}
</script>

<template>
<h1>Home Components {{10+20}}</h1>
<h1>Home Components {{"Hello".length}}</h1>
<h1>Email{{email}}</h1>
<h1>Mobile{{mobile}}</h1>
<h1>Mobile{{mobile==6878}}</h1>
<h1>Name{{getName()}}</h1>
<h1>Names{{getNames("peter")}}</h1>
<h1>Names2{{getNames("kohinur")}}</h1>
<h1>All Data{{getData().emails}}</h1>
</template>

<script>
export default {
    name: 'Home',
    data() {
        return {
            email: "jayavish@gmail.com",
            mobile: 86789867,
            getName: function () {
                return "Jaya Vishwakarma"
            }
        }
    },
    methods: {
        getNames(name) {
            return name
        },
        getData() {
            return {
                name1: "jaya",
                emails: this.email
            }
        }
    }
}
</script>

<style scoped>
h1 {
    color: orange;
}
</style>

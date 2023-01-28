<template>
<h1>Simple Form</h1>
<!-- <p>{{form}}</p> -->
<ul>
    <li v-for="item in error" v-bind:key="item">
        {{ item }} not valid
    </li>
</ul>
<form>
    <lable>Email:</lable>
    <input type="text" placeholder="enter email" v-model="form.email" />
    <br />
    <br />
    <lable>Password:</lable>
    <input type="password" placeholder="enter Password" v-model="form.password" />
    <br /><br />
    <lable>Select Country:</lable>
    <select v-model="form.country">
        <option>India</option>
        <option>China</option>
        <option>USA</option>
        <option>UK</option>

    </select> <br />
    <br />
    <h3>Technology</h3>
    <lable>Java:</lable>
    <input type="checkbox" value="java" v-model="form.technology" />
    <br /><br />

    <lable>React:</lable>
    <input type="checkbox" value="react" v-model="form.technology" />
    <br /><br />

    <h3>Radio</h3>
    <lable>Male:</lable>
    <input type="radio" value="male" v-model="form.gender" />
    <br /><br />

    <lable>Female:</lable>
    <input type="radio" value="female" v-model="form.gender" />
    <br /><br />

    <button v-on:click="login" type="button">LOGIN</button>
</form>
</template>

<script>
export default {
    name: 'SimpleForm',
    data() {
        return {
            form: {
                email: '',
                password: '',
                country: '',
                technology: [],
                gender: ''
            },
            error:[],
        }
    },
    methods: {
        login() {
            this.error=[];
            for(const item in this.form)
            {
                if(this.form[item]==="" || this.form[item].length===0)
                {
                    this.error.push(item)
                }
            }
            if(this.error.length===0){
                alert("succes data submitted")
            }
            console.log("Login data", this.form,this.error)
        }
    }
}
</script>

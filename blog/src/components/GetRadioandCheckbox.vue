<template>
<h1>Get Radio and CheckBox Value</h1>
<h3>Technologies</h3>
<label for="java">Java</label>
<input type="checkbox" value="java" v-model="technology" id="java"/> 
<label for="php">php</label>
<input type="checkbox" value="php" v-model="technology" id="php"/> 
<label for="node">node</label>
<input type="checkbox" value="node" v-model="technology" id="node"/> 
<br/><br/>

<h3>who I am </h3>

<label for="student">Student</label>
<input type="radio" value="student" v-model="names" name="names" id="student"/> 

<label for="developer">Developer</label>
<input type="radio" value="developer" v-model="names" name="names" id="developer"/> 
<br/><br/>
<h4>Selected Technology :{{technology}}</h4>
<h4>I am a :{{names}}</h4>
</template>
<script>
export default{
    name:'GetRadioandCheckbox',
    data(){
        return{
            technology:[],
            names:null
        }
    }
}
</script>
<style>
</style>
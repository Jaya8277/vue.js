<template>
<img alt="Vue logo" src="./assets/logo.png">
<HelloWorld msg="Welcome to Your Vue.js App" />
<Home/>
<Button/>
<GetInput/>
<GetRadioandCheckbox/>
<IfelseCondition/>
<ForLoop/>
<PassDatatochild/>
<ReuseComponnets/>
<HtmlBinding/>
<ClassBinding/>
<Props/>
<Parent/>
<Ref/>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Home from './components/Home.vue'
import Button from './components/Button.vue'
import GetInput from './components/GetInput.vue'
import GetRadioandCheckbox from './components/GetRadioandCheckbox.vue'
import IfelseCondition from './components/IfelseCondition.vue'
import ForLoop from './components/ForLoop.vue'
import PassDatatochild from './components/PassDatatochild.vue'
import ReuseComponnets from './components/ReuseComponnets.vue'
import HtmlBinding from './components/HtmlBinding.vue'
import ClassBinding from   './components/ClassBinding.vue'
import Props from './components/Props.vue'
import Parent from './components/Parent.vue'
import Ref from './components/Ref.vue'

export default {
    name: 'App',
    components: {
        HelloWorld,
        Home,
        Button,
        GetInput,
        GetRadioandCheckbox,
        IfelseCondition,
        ForLoop,
        PassDatatochild,
        ReuseComponnets,
        HtmlBinding,
        ClassBinding,
        Props,
        Parent,
        Ref
    }
}
</script>

<!-- <style>
#app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
}
</style> -->

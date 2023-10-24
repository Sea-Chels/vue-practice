<template>
    <header>
        <h1>{{ title }}</h1>
        <ButtonItem text="Add Task" color="green"/>
    </header>
 </template>
 <script>
 import ButtonItem from './Button.vue'
    export default {
        name: 'HeaderItem',
        // props: ['title'] this is a simple version of defining props with no type checks. 
        props: {
            title: {
                type: String,
                default: 'Hello World' // you can leave it as just props: { title: String } if you want but you can also put in more prop details 
            }
        },
        components: {
            ButtonItem,
        }
    }
</script>
<style scoped>
header {
     display: flex;
     justify-content: space-between;
     align-items: center;
     margin-bottom: 20px;
}
</style>
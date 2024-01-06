<template>
    <h1>This is {{ name }}'s component and {{gender}} callsign is {{ callsign }}</h1>
    <h2>This is my email address: {{ email }}</h2>
    <h2>This is my mobile number: {{ mobile }}</h2>
    <h1>Developer's Full Name: {{ getname('Ajay Joshi') }} address: {{ getAddress() }}</h1>
    <p>customer info: {{ personalInfo().name }}</p>
    <button @click="count=count+10">Alternate mobile no.</button>
    <button >Count: {{ count }}</button>
    <input type="text" v-model="caste">
    <h2>{{ caste }}</h2>
    </template>

<script>
export default {
props: ['name','callsign','gender'],
name: "Mycomp",
data() {
    return {
        email: 'joshiajay311@gmail.com',
        caste: 'EWS',
        mobile: '+91-8586934166',
        count: 0,
        getname: function(arg) {
            return arg
        },
        counter:function() {
        count++;
    }
    }
},
methods:{
    getAddress() {
        return "gole market New delhi-110001"
    },
    personalInfo() {
        return{
            name:"Niel",
            favFood: "Pasta"
        }
    }
}   
}

</script>

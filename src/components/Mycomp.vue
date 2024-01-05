<template>
    <h1>This is {{ name }}'s component and {{gender}} callsign is {{ callsign }}</h1>
    <h2>This is my email address: {{ email }}</h2>
    <h2>This is my mobile number: {{ mobile }}</h2>
    <h1>Developer's Full Name: {{ getname('Ajay Joshi') }} address: {{ getAddress() }}</h1>
    </template>

<script>
export default {
props: ['name','callsign','gender'],
name: "Mycomp",
data() {
    return {
        email: 'joshiajay311@gmail.com',
        mobile: '+91-8586934166',
        getname: function(arg) {
            return arg
        }
    }
},
methods:{
    getAddress() {
        return "gole market New delhi-110001"
    }
}
}
</script>

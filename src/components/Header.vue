<template>
<header>
    <img 
        @click="reload"
        src="https://drive.google.com/uc?export=download&id=14Eud0Uy8ymq_C7WhjQTyK3g1KBAiFUH2" 
        alt="Logo"
    />
    <h1><span>Cash</span>Flow</h1>
    <span></span>
</header>
</template>

<script>
export default{
    methods:{
        reload(){
            location.reload();
        }
    }
}
</script>


<style>
@import '../assets/css/Header/header.css';
</style>
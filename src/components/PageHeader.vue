<script>
export default {

}
</script>

<template>
    <div class="header">
        <div class="header-items header-left">
            <a href="/index.html"><img id="logo" src="../assets/logo.png"></a>
            <button class="header-link nav" >Mani pirkumi</Button>
            <button class="header-link nav" >Mans profils</button>
            <button class="header-link nav" >Piedāvājums</button>
        </div>
        <div class="header-items header-right">
            <!--<img class="header-profile" src="../assets/img/rat.jpg"></img>-->
            <button class="header-link login" href="/login.html">Login</button>
            <button class="header-link signup" href="/signup.html">Sign up</button>
        </div>
    </div>
</template>

<style>
#logo {
    height: 40px;
    margin-bottom: 6px;
}
.header {
    position:fixed;
    top: 0;
    left: 0;
    z-index: 10;
    display: flex;
    width: 100%;
    background-color: #05442f;
    height: 60px;
    justify-content: space-between;
    padding-left: 20px;
}
.header-link {
    margin-left: 10px;
}
.nav {
    margin-bottom: 0;
    margin-left:20px;
    padding: 15px;
    border-radius: 15px;
    border-bottom-left-radius: 0;
    border-bottom-right-radius: 0;
    background-color: #05442f;
    border: solid #bdf2e2 2px;
    color: #bdf2e2;
    border-bottom: 0;
}
.login {
    background-color: #bdf2e2;
}
.signup {
    background-color: #1b5c47;
    color: #bdf2e2;
    border: solid #bdf2e2 1px;
}
.header-items {
    display: flex;
    align-items: center;    
}
.header-left {
    align-items: flex-end;
}
.header-right {
    justify-content: end;
    margin-right: 30px;
}
.header-profile {
    object-fit: cover;
    height: 40px;
    width: 50px;
    border-radius: 50%;
    margin:0;
}
</style>
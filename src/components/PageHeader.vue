<script>
export default {

}
</script>

<template>
    <div class="header">
        <div class="header-items header-left">
            <a href="/index.html"><img id="logo" src="../assets/logo.png"></a>
            <a class="header-link" href="/profils.html">Mani pirkumi</a>
            <a class="header-link" href="/profils.html">Mans profils</a>
            <a class="header-link" href="/profils.html">Piedāvājums</a>
        </div>
        <div class="header-items header-right">
            <a class="header-link" href="/login.html">Login</a>
            <a class="header-link" href="/signup.html">Sign up</a>
        </div>
    </div>
</template>

<style>
#logo {
    height: 40px;
}
.header {
    position:fixed;
    top: 0;
    left: 0;
    display: flex;
    width: 100%;
    background-color: #2e2e2e;
    height: 40px;
    justify-content: space-between;
    padding: 10px;
    padding-left: 20px;
}
.header-link {
    padding: 5px;
}
.header-items {
    display: flex;
    align-items: center;    
}
.header-right {
    justify-content: end;
    margin-right: 30px;
}
</style>
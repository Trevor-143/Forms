<template>
    <main>
        <h1>Hello World</h1>



        <button> <router-link to="./login">Log-Out</router-link> </button>
    </main>
</template>

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
a {
    color: #ffffff;
}
a:hover {
    color: #100385;
}
body {
    align-items: center;
    justify-content: center;
    height: 100vh;
    display: flex;
    text-align: center;
}
button {
    border: none;
    background: #100385;
    color: #ffffff;
    padding: 15px 25px;
    border-radius: 6px;
    transition: 0.4s;
}
button:hover {
    background: #ffffff;
}

</style>
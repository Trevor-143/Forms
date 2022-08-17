<template>
    <main>
        <header>
            <h1  class="logo">L.E.G.E.N.D.A.R.Y</h1>


            <h2>Log-in</h2>
            <p>Login to enter Lengendary</p>
        </header>

        <form @submit.prevent>
            <label>
                <span>Email Please</span>
                <input type="email" v-model="email" placeholder="email">
            </label>
            <label>
                <span>Password Please</span>
                <input type="password" v-model="password" placeholder="************">
            </label>

            <button type="submit">Enter</button>
        </form>


        <footer>
            <p>Dont have an account? <router-link to="/register">Register</router-link></p>
        </footer>
    </main>
</template>

<script>

    import { ref } from 'vue'

    const email = ref('')
    const password = ref('')

</script>



<style scoped>
main {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-between;
    height: 100vh;
    padding: 20px 0;
}

header {
    display: flex;
    flex-direction: column;
    text-align: center;
}
form {
    min-width: 500px;
    background: #e0e0ff;
    border: none;
    border-radius: 10px;
    display: flex;
    flex-direction: column;
    padding: 30px;
}
label {
    display: flex;
    flex-direction: column;
    margin: 5px 0;
}
label span {
    margin: 10px 0;
}
button {
    padding: 10px 20px;
    border: none;
    color: #ffffff;
    background: #0b0470;
    border-radius: 10px;
    width: fit-content;
    cursor: pointer;
    transition: 0.4s;
}
button:hover {
    color:#0b0470;
    background: #ffffff;
}
</style>
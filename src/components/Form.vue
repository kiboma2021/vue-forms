<template>
  <form>
    <div>
        <label>Name</label>
        <input type="name" v-model="name">
    </div>

    <div>
        <label>Email</label>
        <input type="email" v-model="email">
    </div>


    <div>
        <label>Password</label>
        <input type="password" v-model="password">
    </div>


  </form>
</template>

<script>
export default {
    data() {
        return {
            name: "Ben",
            email: "admin@localhost.com",
            password: "password1!"
        }
    }

}
</script>

<style>

label {
    margin: 1rem;
    font-weight: bold;
    padding: 1rem;
}
input {
    border: none;
    width: 12rem;
    height: 1rem;
    margin: 1rem;
    padding: 1rem;
}

</style>
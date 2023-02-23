<template>
  <form>
    <div>
        <label>Name</label>
        <input type="name" v-model="name" required>
    </div>

    <div>
        <label>Email</label>
        <input type="email" v-model="email" required>
    </div>


    <div>
        <label>Password</label>
        <input type="password" v-model="password" required>
    </div>

    <button type="submit" >Submit</button>
  </form>

  <p>Name: {{ name }}</p>
  <p>Email: {{ email }} </p>
  <p>Password: {{ password }}</p>
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
<template>
  <form>
    <div>
        <label>Name</label>
        <input type="name">
    </div>

    <div>
        <label>Email</label>
        <input type="email">
    </div>


    <div>
        <label>Password</label>
        <input type="password">
    </div>


  </form>
</template>

<script>
export default {
    

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
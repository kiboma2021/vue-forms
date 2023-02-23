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
    
    <div>
        <label>Role</label>
        <select v-model="role" required>
            <option value="developer">Web Developer</option>
            <option value="designer">Web Designer</option>
            <option value="engineer">Backend Engineer</option>
        </select>
    </div>

    <div class="terms">
        <input type="checkbox" v-model="terms" required>
        <label>Accepts terms and conditions</label>
    </div>



    <br> <br>
    <button type="submit" >Submit</button>
  </form>

  <p>Name: {{ name }}</p>
  <p>Email: {{ email }} </p>
  <p>Password: {{ password }}</p>
  <p>Role: {{ role }}</p>
  <p>Accept Terms: {{ terms }}</p>
</template>

<script>
export default {
    data() {
        return {
            name: "",
            email: "",
            password: "",
            role: "developer",
            terms: false,
        }
    }

}
</script>

<style>

form {
    max-width: 420px;
    margin: 30px auto;
    background: white;
    text-align: left;
    padding: 40px;
    border-radius: 10px;
}
label {
    color: #aaa;
    display: inline-block;
    margin: 25px 0 15px;
    font-size: 0.6em;
    text-transform: uppercase;
    letter-spacing: 1px;
    font-weight: bold;
}
input,select {
    display: block;
    padding: 10px 6px;
    width: 100%;
    box-sizing: border-box;
    border: none;
    border-bottom: 1px solid #ddd;
    color: #555;
}

input[type="checkbox"] {
    display: inline-block;
    width: 16px;
    margin: 0 10px 0 0;
    position: relative;
    top: 2px;
}

</style>
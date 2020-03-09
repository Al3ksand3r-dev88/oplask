<template>
    <div class="container">
        <h1>Oplask</h1>
        <form>
            <input type="text" class="input">
            <button class="submit">
            <i class="fas fa-search"></i>
            </button>
        </form>
    </div>
</template>

<script>
    export default {
        name: 'Search',
        
    }
</script>

<style lang="scss" scoped>
.container {
   width: 800px;
   margin: auto;

}
form {
  position: relative;  
  display: flex;
}
input[type="text"] {
  top: 10px;  
  width: 640px;
  padding: 15px;
  border: 2px solid grey;
  outline: 0;
  border-radius: 2rem;
  
}

button{
  top: 0;
  right: 120px;  
  position: absolute;
  color: #000;
  border: 2px grey solid;
  cursor: pointer;
  border-radius: 2rem;
  padding: 15px;
    
}
.submit{
        color:#000;
    }
</style>
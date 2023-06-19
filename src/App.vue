<template>
  <header>
    <nav class="menu">
      <img src="./assets/logo.png" alt="logo" class="foto">
      <ul class="linking">
        <li class="list-pro">
          <a href="/">HOME</a>
        </li>
        <li class="list-pro">
          <a href="/profile">PROFILE</a>
        </li>
      </ul>
      <form class="d-flex" role="search">
        <input class="pesquisa" type="search" placeholder="Search" aria-label="Search">
      </form>
    </nav>
  </header>
  <body></body>
  <router-view/>
</template>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Play:wght@700&display=swap');
@import url('https://fonts.googleapis.com/css2?family=M+PLUS+1:wght@500&display=swap');

header{
  padding: 0px;
  margin: 0px;  
  background-color: #121212;
}
form {
  display: inline-block;
}
.menu{
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 10px;
  background-color: #121212;
  width: auto;
  margin: 0px;
}
*{
  box-sizing: border-box;
  margin: 0;
  padding: 0;
  background-color: #0d0d0d;}
.list-pro, a {
  background-color: #121212;
  font-family: 'Play', sans-serif;
  text-decoration: none;
  font-weight: 700;
  font-size: 25px;
}
ul, .list-pro{
  background-color: #121212;
}

.foto{
height: 50px;
width: 150px;
background-color: #121212;
cursor: pointer;
}
.about{
  font-size: medium;
}
.linking{
  list-style: none;
  display: inline-block;
  padding: 0px 20px;
}
.linking li{
  display: inline-block;
  padding: 0px 20px;
}
.linking li a{
  transition: all 0.3s ease 0s;
}

.linking li a:hover{
  font-size: larger;
color: rgb(31, 167, 31);
}
.pesquisa {
  border: none;
  outline: none; 
  padding: 10px; 
  color: rgb(27, 27, 27);
  background-color: #424242; 
  background-position: right center;
  background-size: 20px; 
  border-radius: 10px;
  opacity: 0.4;
  box-shadow: 0 2px 4px;
  font-family: 'Play', sans-serif;
}

</style>

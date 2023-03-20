<script setup>
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>

  <header>
    <div class="wrapper">
      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
        <RouterLink to="/contact">Contact</RouterLink>
      </nav>
    </div>
  </header>

  <RouterView />
</template>

<style >

:root {
  --background :#202020;
  --link-aktivt: aqua;
  --link: rgb(0, 174, 174);
  --grey:rgb(136, 136, 136);
}


*{
  font-family: 'Roboto', sans-serif;
  color: white;

}

body{
  background-color:var(--background);
  padding: 2rem 5rem;
}

header {
  line-height: 1.5;
  display: flex;
  place-items: right;

}

nav {
  width: 100%;
  font-size: 20px;
  text-align: center;
  background: transparent;
  box-shadow: 0px 1px 0px 0px var(--link-aktivt);
  font-size: 25px;

}

nav a.router-link-exact-active {
  color:var(--link-aktivt);
  
}

nav a:hover {
  color:var(--link-aktivt);
}

nav a {
  display: inline-block;
  padding-right: 1rem;
  border-left: 1px solid var(--color-border);
  text-decoration: none;
  color: var(--link);
  
  
  
}

.presentation{
  border-style: solid;
  border-color: var(--background) var(--link);
  height: 600px;
}

.presentation:nth-child(2){
  margin-top: 50px;
  border-style: solid;
  border-color: var(--link) var(--background);
  height: 500px;
}
.presentation h1{
  margin: 0;
  position: absolute;
  top: 40%;
  left: 50%;
  transform: translate(-80%, -50%);
  font-size: 75px;
  line-height: 3cm;

}

.h2pre{
  margin: 0;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-60%, -50%);
  font-size: 50px;
  line-height: 3cm;
  color: var(--grey);
}
.intro{
  width: 50%;
  float: left;
  margin-left: 100px;
}

.intro img{
  width: 100px;

  padding-top: 50px;
}

.lan1{padding-left: 15%;}

.lan2{padding-left: 15%;}

.lan3{padding-left: 0;}

.lan4{padding-left: 15%;}

.lan5{padding-left: 15%;}

.lan6{padding-left: 15%;}

.lan7{padding-left: 15%;}


.intro2{
  width: 40%;
  padding-top:100px ;
  float: right;
}
.intro2 h3{
  font-size: 50px;
}
.intro2 p{
  font-size: 20px;
}

.profilePic{
  width: 30%;
  transform: translate(220%, 20%);
  opacity: 0.7; 
  -webkit-filter: grayscale(100%); /* Safari 6.0 - 9.0 */
  filter: grayscale(100%);
  border-radius: 50%;
  
  
}
.some {
  width: 50px;
  transform: translate(0, 350%);
  margin-right: 3rem;
  float: right;
  
}

/* About me */ 

.h2abo{
  text-align: center;
  font-size: 50px;
  
}
.aboutpre{
  padding: 0 10%;
}

.presentation section{
  display: flex;
  text-align: center;
  padding: 10% 10%;
}

.cards{
  width: 33%;
  border: 1px solid white;
  border-radius: 5px;
  margin: 0 10px;
}
.cards img{
  width: 100%;
}

/* Contact */




#title-Tag-Line {
  font-size: 20px;
}


/* form animation starts */
.form {
  background: #fff;
  box-shadow: 0 15px 30px 0 var(--link-aktivt);
  border-radius: 5px;
  max-width: 480px;
  margin-top: 5%;
  margin-left: auto;
  margin-right: auto;
  padding-top: 5px;
  padding-bottom: 5px;
  left: 0;
  right: 0;
  position: absolute;
  border-top: 5px solid var(--link);
/*   z-index: 1; */
  animation: bounce 3s infinite;
}
::-webkit-input-placeholder {
  font-size: 1.3em;
}

.title{
  display: block;
  font-family: sans-serif;
  margin: 10px auto 5px;
  width: 300px;
}
.termsConditions{
  margin: 0 auto 5px 80px;
}

.pageTitle{
  font-size: 2em;
  font-weight: bold;
}
.secondaryTitle{
  color: grey;
}

.name {
  background-color: #ebebeb;
  color: black;
}
.name:hover {
  border-bottom: 5px solid var(--link);
  height: 30px;
  width: 380px;
  transition: ease 0.5s;
}

.email {
  color: black;
  background-color: #ebebeb;
  height: 2em;
}

.email:hover {
  border-bottom: 5px solid var(--link);
  height: 30px;
  width: 380px;
  transition: ease 0.5s;
}

.message {
  color: black;
  background-color: #ebebeb;
  overflow: hidden;
  height: 10rem;
}

.message:hover {
  border-bottom: 5px solid var(--link);
  height: 12em;
  width: 380px;
  transition: ease 0.5s;
}

.formEntry {
  display: block;
  margin: 30px auto;
  min-width: 300px;
  padding: 10px;
  border-radius: 2px;
  border: none;
  transition: all 0.5s ease 0s;
}

.submit {
  width: 200px;
  color: white;
  background-color: var(--background);
  font-size: 20px;
}

.submit:hover {
  box-shadow: 15px 15px 15px 5px rgba(78, 72, 77, 0.219);
  transform: translateY(-3px);
  width: 300px;
  border-top: 5px solid #0e3750;
  border-radius: 0%;
}

@keyframes bounce {
  0% {
    tranform: translate(0, 4px);
  }
  50% {
    transform: translate(0, 8px);
  }
} 




@media only screen and (max-width: 900px) {
.profilePic{
  display: none;
}

.intro{
  display: none;
}

.intro2{
  width: 100%;
  padding-top:50px ;
  float: none;
}
.intro2 h3{
  font-size: 40px;
}
.intro2 p{
  font-size: 25px;
}

.some {
display: none;
}

body{
  background-color:var(--background);
 
}

}
  
@media only screen and (max-width: 1200px) {

.presentation h1{
  margin: 0;
  position: absolute;
  top: 10%;
  left: 15%;
  transform: translate(0, 0);
  font-size: 50px;

}
.h2pre{
  margin: 0;
  position: absolute;
  top: 15%;
  left: 15%;
  transform: translate(0, 0);
  font-size: 30px;
  line-height: 3cm;
  color:rgb(136, 136, 136);
}

.intro{
  width: 50%;
  float: left;
  margin-left: 80px;
}
.intro img{
  width:80px;

  padding-top: 50px;
}
.intro2{
  width: 100%;
  padding-top:0px ;
  float: none;
}

.intro2 h3{
  font-size: 40px;
}
.intro2 p{
  font-size: 20px;
}

}
@media only screen and (max-width: 1300px) {

  body{
  background-color:var(--background);
  padding: 2rem 2rem;
}
}

</style>

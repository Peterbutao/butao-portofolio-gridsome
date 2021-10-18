<template>

<section class="layout">
  <nav>
    <div class="navigation">

      <div class="brand">
        <h1>
          <g-link to="/">{{ $static.metadata.siteName }}</g-link>
          
        </h1>
      </div>

      <div :class="{'clip': toggle}" class="navlist">
        <ul >
          <li >
            <g-link>About</g-link>
          </li>
          <li>
            <g-link>Work</g-link>
          </li>
          <li>
            <g-link>Contact</g-link>
          </li>
         
        </ul>
      </div>

      <div @click="toggle = !toggle" class="toggle">
        <div class="line-1"></div>
        <div class="line-2"></div>
        <div class="line-3"></div>
      </div>

    </div>
  </nav>

  <main>
    <slot/>
  </main>
  <footer>
    <Footer />
  </footer>
</section>



</template>

<static-query>
query {
  metadata {
    siteName
  }
}
</static-query>
<script>
import Footer from "../lib/Footer.vue"
export default {
  data(){
    return {
      toggle: false
    }
  },
  components: {
    Footer
  }
}
</script>
<style>
:root{
  --pm: #665e5e;
  --pc:#E1CFCF;
  --wc: seashell;
  --tc: black;
  --mw: 760px;
  --nbg: rgba(255, 255, 255, 0.534);

}
.color{
  color: red !important;
}
body {
  font-family: -apple-system,system-ui,BlinkMacSystemFont,"Segoe UI",Roboto,"Helvetica Neue",Arial,sans-serif;
  margin:0;
  padding:0;
  box-sizing: border-box;
  line-height: 1.5;
}
.brand > h1 {
  font-weight: 500;
}

nav{
  background: var(--nbg);
  position: fixed;
  width: 100%;
  top: 0;
  left: 0;
  z-index: 99;
}
.navigation {
  max-width: var(--mw);
  margin:auto;
  display: flex;
  justify-content: space-between;
  align-items: center;
 
}

.navlist {
  margin-left: 20px;
}
ul{
  list-style: none;
  padding: 0;
  margin:0;
  display: flex;

}
li{
    margin-left: 15px;
    padding:0;
}
a{
  text-decoration: none;
  color: var(--tc);
}
.toggle{
  display: none;
}
@media screen and (max-width: 700px) {
  .clip{
        -webkit-clip-path: circle(1000px at 90%) !important;
    clip-path: circle(1000px at 90%) !important;
    pointer-events: all !important;
    transition: all ease 1s;

  }
  nav{
    position: relative;
    
  }
  .navlist{
    position: fixed;
    height: 100vh;
    width: 100%;
    left:0;
    bottom:0;
    margin:0;
    background: var(--pc);
    display: flex;
    align-items: center;
    justify-content: center;
    -webkit-clip-path: circle(0px at 90%);
    clip-path: circle(0px at 90%);
    pointer-events: none;
    transition: all ease 1s;
    
  }
  ul{
    flex-direction: column;
    align-items: center;
    width: 100%;
    
    
  }
  
  .navlist > ul > li{
    width: 100%;
    text-align: center;
    padding: 20px 0;
    
    
  }
  .navlist > ul> li > a{
    padding: 20px;
    font-size: 1rem;
    
  }
  .brand{
    z-index: 99;
  }
  
  .toggle{
    display: block !important;
    padding: 10px;
    z-index: 99;
  }
  .line-1,.line-2,.line-3 {
    background: var(--tc);
    height: 3px;
    width: 25px;
    border-radius: 4rem;
    margin: 3px 0px;
  }

}
</style>

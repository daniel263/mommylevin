<template>
<meta name="viewpoint" content="width=width-device-width, initial-scale=1.0">

  <div id="nav">
   <span> Mommy_Levin Cakes   |    </span> 
    <router-link :to="{name: 'Home'}">Home</router-link> |
    <router-link :to="{name: 'About'}">About</router-link> |
    <router-link :to ="{name:'Cakegallery'}">Cake Gallery</router-link>
  </div>
  <router-view/>
  

  <footer class="footer">
    <div class="container">
      <div class="row">
        <div class="footer-col">
          <h4>Contact Us on:</h4>
      
            <ul>
                <li><img src="./assets/phone-call.svg" alt="Call us on" width="20" height="20" margin-top="15"> {{phone2}}</li>   
                <li><img src="./assets/whatsapp.svg" alt="Whatsapp us on" width="20" height="20" margin-bottom="5"> {{phone}} </li>    
                <li> <img src="./assets/email.svg" alt="Email us on" width="20" height="20" margin-bottom="5"> {{email}} </li>  
                <li><img src="./assets/map.svg" alt="We are located at " width="20" height="20" margin-bottom="5"> {{address}}  </li>
                
            </ul>
      
        </div>
        <div class="footer-col">
          <h4>Copyright</h4>
         <p> {{copy}} &copy</p>
        </div>
        <div class="footer-col">
          <h4>PoweredBy</h4>
         <p> <img src="./assets/thunderbolt.png" alt="powerup" width="20" height="20" margin-bottom="5"> {{signed}}</p>
        </div>
      </div>
    </div>

   

        
                
    </footer>
</template>
<script>


export default{
  data(){
    return{
         phone:'+263 776 310 659',
        phone2: '+263 719 310 659',
        email: 'gracebasvi03@gmail.com',
        address: '4268 152 Street Warren Park D, Harare',
        signed: 'Mshaty263',
        copy:'Mommy Levin Cakes 2021'
    }
  }
  
}
</script>


<style>

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #111;
}

#nav {
  padding: 5px;
  text-decoration: none;
  justify-content: space-between;
  text-align: center;
  letter-spacing: 1px;
  font-family: 'comic neue';

}

#nav a {
  font-weight: normal;
  font-size: 1.2em;
  color: #3d2827;
  text-decoration: none;
  
}
#nav a:hover{
  font-weight: bold;
  color: #f00e56
}


#nav a.router-link-exact-active {
  color: #f00e56;
}
#nav span{
  color:#f00e56;
  font-weight: bold;
  font-family: Pacifico;
  font-size: 1.2em;
  }
  footer{
    font-size: 15px;
    text-align: start;
    color:rgb(6, 41, 41);
    background:rgb(236, 234, 234);
    height: 100%;
    margin-left:15px;
    font-family: ubuntu;
    
}
footer .row{
  display: flex;
  flex-wrap: wrap;
}
footer li{
    list-style: none;
    font-size:15px;
    font-weight: normal;
    justify-content: space-between;

    
    
}
footer .footer-col{
  width: 25%;
  padding: 00 15px;
}
.footer-col h4 {
  font-size:18px;
  text-transform: uppercase;
  position: relative;
  font-weight: 500x;
}
.footer-col h4::before{
  content:'';
  position: absolute;
  left:0;
  bottom: -10px;
  background-color: rgb(6, 41, 41);
  height: 2px;
  box-sizing: border-box;
  width:50%;

}
@media(max-width:991px){
  #nav{
    text-align:end;
    font-size:10px;
  }
  section{
      padding: 20px;
  }
  .content{
    flex-direction: column;
    padding:10px;
    margin-bottom: 15px;
  }
  .content .textbox{
    margin-bottom: 25px;
    max-width: 100%;
  }
  .content .imgbox{
    max-width: 100%;
  }
  .content .imgbox img{
    max-width:250px;
  }
  .circle1{
    position:absolute;
    top:0;
    left: 0;
    width:100%;
    height: 100%;
    background: #f00e56;
    clip-path: circle(100px at left 100px)
}

}
footer {
  font-size: 15px;
}
</style>

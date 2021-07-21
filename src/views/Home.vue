<template> 

<section>
<div class="circle"></div>
<div class="circle1"></div>
<div class="content">
  <div class="textbox">
    <h2>Just Name Your Flavour <br><span>We Cake IT</span>  </h2>
    <p>Cakes for All Events
      
    </p>
    <router-link :to="{name:'Cakegallery'}">View our Cakes </router-link>
  </div>
  <div class="imgbox">
    <img src="../assets/slice.jpeg" alt="Cake Slice" width="400" height="400" >
  </div>
</div>
</section>

</template>

<script>


export default {
}
</script>
<style scoped>
*{
  font-family:ubuntu;

 
}
section{
  margin-top: -50px;

  min-height: 100%;
  padding:100px;
  display: flex;
  justify-content: space-between;
  align-items:center;
  background:#fff; 

}
.content{
  position: relative;
  width: 100%;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.content .textbox{
  position:relative;
  max-width: 800px;
  margin-left: 250px;
}
.content .textbox h2{
  color: #1ca1f8;
  font-size: 2em;
  line-height: 1.3em;
  font-weight: 300px;
  
}
.content .textbox h2 span{
  color:rgba(235, 201, 8, 0.911);
  font-size: 1em;
  font-weight: 400;
  border-radius: 5px;
  
}
.content .textbox p
{
  color: #333;
  font-size: 1em;

}

.content .textbox a{
  display: inline-block;
  margin-top: 20px;
  padding: 8px 20px;
  background:#3d2827;
  color:#fff;
  border-radius:8px;
  text-decoration: none;
  letter-spacing: 1px;
}
.content .textbox a:hover{
  font-weight: bold;
  background-color: #f00e56;
  font-size: 1.1em;
  letter-spacing: 2px;
}
.content .imgbox{
  width:300px;
  display:flex;
  justify-content: flex-end;
  
}
.content .imgbox img {
  border-radius:80px;
  max-width: 500px;

}
.circle{
position:absolute;
top:0;
left: 0;
width:100%;
height: 100%;
background: #f00e56;
clip-path: circle(400px at right 800px);
}
.circle1{
position:absolute;
top:0;
left: 0;
width:100%;
height: 100%;
background: #f00e56;
clip-path: circle(300px at left 100px);


}

@media (max-width:991px){
  #nav{
    font-size: 15px;
  }
.circle{
position:absolute;
top:0;
left: 0;
width:100%;
height: 100%;
background: #f00e56;
clip-path: circle(200px at right 500px);
}
.circle1{
position:absolute;
top:0;
left: 0;
width:100%;
height: 100%;
background: #f00e56;
clip-path: circle(100px at left 110px);
}
.content .textbox{
  position:relative;
  max-width: 800px;
  margin-left:5px ;
}
.content .textbox h2{
  color: #1ca1f8;
  font-size: 1.3em;
  line-height: 1.3em;
  font-weight: 80px;
  
}
.content .textbox a{
  display: inline-block;
  margin-top: 10px;
  padding: 5px 5px;
  background:#3d2827;
  color:#fff;
  border-radius:8px;
  text-decoration: none;
  font-size: 15px;
  
}
.content .textbox a:hover{
  font-weight: bold;
  background-color: #f00e56;
  font-size: 20px;
  letter-spacing: 1px;
}
}
</style>

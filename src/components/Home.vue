<template>

<div>

   
   <hooper id = "hoopers" :settings="hooperSettings">
      <slide>
        <div class="images">
          <img src="https://picsum.photos/1600/700/?image=28" style="height:110vh;width:100%">
        </div>
      </slide>
      <slide>          
        <div class="images">
          <img src="https://picsum.photos/1600/700/?image=39" style="height:110vh;width:100%">
        </div> 
      </slide>
      <slide>          
        <div class="images">
          <img src="https://picsum.photos/1600/700/?image=32" style="height:110vh;width:100%">
        </div>       
      </slide>
      <slide>  
        <div class="images">
          <img src="https://picsum.photos/1600/700/?image=21" style="height:110vh;width:100%">
        </div> 
      </slide>
      <slide>     
        <div class="images">
          <img src="https://picsum.photos/1600/700/?image=22" style="height:110vh;width:100%">
        </div>
      </slide>
        <hooper-navigation slot="hooper-addons">
      <svg slot="hooper-prev" class="svg-icon" viewBox="0 0 20 20" width="60px" height="60px" fill="gray">
        <path d="M11.739,13.962c-0.087,0.086-0.199,0.131-0.312,0.131c-0.112,0-0.226-0.045-0.312-0.131l-3.738-3.736c-0.173-0.173-0.173-0.454,0-0.626l3.559-3.562c0.173-0.175,0.454-0.173,0.626,0c0.173,0.172,0.173,0.451,0,0.624l-3.248,3.25l3.425,3.426C11.911,13.511,11.911,13.789,11.739,13.962 M18.406,10c0,4.644-3.763,8.406-8.406,8.406S1.594,14.644,1.594,10S5.356,1.594,10,1.594S18.406,5.356,18.406,10 M17.521,10c0-4.148-3.373-7.521-7.521-7.521c-4.148,0-7.521,3.374-7.521,7.521c0,4.148,3.374,7.521,7.521,7.521C14.147,17.521,17.521,14.148,17.521,10"></path>
      </svg>
      <svg slot="hooper-next" class="svg-icon" viewBox="0 0 20 20" width="60px" height="60px" fill="gray">
        <path d="M12.522,10.4l-3.559,3.562c-0.172,0.173-0.451,0.176-0.625,0c-0.173-0.173-0.173-0.451,0-0.624l3.248-3.25L8.161,6.662c-0.173-0.173-0.173-0.452,0-0.624c0.172-0.175,0.451-0.175,0.624,0l3.738,3.736C12.695,9.947,12.695,10.228,12.522,10.4 M18.406,10c0,4.644-3.764,8.406-8.406,8.406c-4.644,0-8.406-3.763-8.406-8.406S5.356,1.594,10,1.594C14.643,1.594,18.406,5.356,18.406,10M17.521,10c0-4.148-3.374-7.521-7.521-7.521c-4.148,0-7.521,3.374-7.521,7.521c0,4.147,3.374,7.521,7.521,7.521C14.147,17.521,17.521,14.147,17.521,10"></path>
      </svg>
        </hooper-navigation>
        
        <hooper-pagination slot="hooper-addons"></hooper-pagination>
    </hooper>

    

</div>
</template>
<script defer src="https://use.fontawesome.com/releases/v5.0.10/js/all.js" integrity="sha384-slN8GvtUJGnv6ca26v8EzVaR9DC58QEwsIk9q1QXdCU8Yu8ck/tL/5szYlBbqmS+" crossorigin="anonymous"></script>

<script>
 import { Hooper, Slide , Pagination as HooperPagination , Navigation as HooperNavigation} from 'hooper';
 import 'hooper/dist/hooper.css';
  

export default {
  name: 'Home',
  components: {
      Hooper,
      Slide,
      HooperPagination,
      HooperNavigation
    },
  data () {
    return {
      hooperSettings: {
          infiniteScroll: true,
          centerMode: true,
          autoPlay: true,
          playSpeed: 1000,
          wheelControl:false,
          
      },
      
      
    }

    
  }
}
</script>

<style>
.images {
  height: 70vh;
  display: flex;
  align-items: center;
  justify-content: center;
  border-radius: 20px;
}
h2 {
  color: #fff
}
#hoopers {
  height: 95vh;
}

.footer {
   
   left: 0;
   bottom: 0;
   width: 100%;
   height: 350px;
   background-color: rgb(3, 91, 162);
   color: white;
   
}

.footer .logo {
    margin-top : 30px;

}

.footer .footer-text{
  padding-top:10px;
  width:50%;
  margin-right:0px;
  float: left;
}

.footer .footer-icon{
  padding-top:10px;
  width:30%;
  margin-right:0px;
  float: right;
}

.footer-icon .icon{
      margin-right:5px;
}
</style>

<!-- Add "scoped" attribute to limit CSS to this component only -->

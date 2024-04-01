<template>

<div class="container1" id="home">

    <div class="item1">
        <div class="box box1">
            <h1 style="font-weight: bold;">Front End Developer</h1>
            <p>I like to make beautiful user interface, it is to have a great user experiences.</p>
        </div>

        <div class="box box2">
            <img src="/images/me.jpg" >
        </div>
    </div>
</div>
</template>

<style scoped>

@import url('https://fonts.googleapis.com/css2?family=Roboto:ital,wght@0,100;0,300;0,400;0,500;0,700;0,900;1,100;1,300;1,400;1,500;1,700;1,900&display=swap');

*{
  padding: 0;
  margin: 0;
}
.container1{
      min-height: 100vh;
      min-width: 100vw;
      background: #5755FE;
      overflow: hidden;
    } 
.box{
    margin: 200px 20px;
}
.item1{
  display: flex; 
  margin-left: 300px;
}

.box1{
  margin-right:  100px;
  width: 350px;
}
.box2{
  margin-left:  100px;
}
img{
  width: 400px;
}
p{
  font-family: "Roboto", sans-serif;
  font-weight: 400;
  font-style: normal;
  margin-top: 30px;
  color: white;
}
h1{
  font-family: "Roboto", sans-serif;
  font-weight: 400;
  font-style: normal;
  font-size: 52px;
  color: #FFC94A;
}

  @media(max-width: 1024px){

  .box1{
    margin-left: -200px;
  }
  img{
    width: 300px;
  }

  }

  @media(max-width: 820px){

  .box1{
    margin-left: -280px;
  }
  img{
    width: 300px;
  }

  }

  @media(max-width: 768px){

  .box1{
    margin-left: -280px;
  }
  img{
    width: 300px;
  }

  }

  @media (max-width: 750px) {
    .item1{
      display: flex;
      flex-direction: column;
    
    }
    .container1{
      min-height: 150vh;
    }
    .box{
      position: absolute;
      left: 20%;
    }
    .box1{
      position: absolute;
      margin: 100px 80px;
    }
    .box2{
      position: absolute;
      margin-top: 400px;
      margin-left: 40px;
    }

    @media(max-width: 540px){

    .box1{
      margin-left: 50px;
    }
    img{
      width: 300px;
    }

    }

    @media(max-width: 430px){

    .box1{
      margin-left: -60px;
    }
    img{
      width: 200px;
    }

    }

    @media(max-width: 414px){

    .box1{
      margin-left: -60px;
    }
    img{
      width: 200px;
    }

    }

    @media(max-width: 375px){

      .box1{
        margin-left: -60px;
      }
      img{
        width: 200px;
      }

    }

    @media(max-width: 280px){
    .container1{
      min-width: 150vw;
    }
    .box1{
      margin-left: -50px;
    }
    img{
      margin-left: -50px;
      width: 200px;
    }

    }
    
}

</style>

<script setup>

</script>
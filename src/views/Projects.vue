<template>

    <div class="container2" id="about">

        <div class="inner-box">

            <div class="box box1">
                <img src="/images/post-test.png" style="">

                <p style="padding: 20px;">I do 3d modelling for rendering and for my dream game 
                    that I will going to make. I want to make a game because I want people to experience
                    playing a game that they never have experience before.</p>

            </div>

            <div class="box box1 second">

               <img src="/images/a.png">

               <p style="padding: 20px">I do anime 2D art also because when I was a kid I always watch anime
                                        and I always wanted to draw anime, and now I am older, I want to make
                                        now an anime style game.
            </p>

            </div>
            <div class="box box1 third">

               <img src="../../public/images/captsone.png">

               <p style="padding: 20px">
                    Web development is fun and I do a little bit of backend development, but the one that
                    I really like to do is front end development because it is a lot of fun, and I enjoy
                    creating a user interface that looks attractive and front end development is close to
                    creating art in games.
                </p>

            </div>


        </div>



    </div>

</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Roboto:ital,wght@0,100;0,300;0,400;0,500;0,700;0,900;1,100;1,300;1,400;1,500;1,700;1,900&display=swap');

.container2{
    min-height: 100vh;
    background: #DDDDDD;
    padding: 30px;
}
.inner-box{
    font-family: "Roboto", sans-serif;
    font-weight: 400;
    font-style: normal;
    background: white;
    padding: 30px;
    border-radius: 20px;
    display: flex;
    justify-content: center;
    margin-top: 100px;
    letter-spacing: 1px ;
    text-align: justify;
    
}
img{
    width: 400px;
    height: 400px;
    border-top-left-radius: 10px;
    border-top-right-radius: 10px;

}
.box{
    border-radius: 10px;
    box-shadow: 10px 10px 5px #aaaaaa;
}
.box1{
    margin: 0 10px;
}
.box2{
    margin-top: 30px;
}
.label{
    font-weight: bold;
    color: gray;
}
.info{
    color: #607274;
}

@media(max-width: 1292px){
    .box{
        width: 300px;
    }
    img{
        width: 300px;
    }
}
@media(max-width: 1024px){
    img{
        width: 250px;
        
    }
    .box{
        width: 280px;
    }
}
@media(max-width: 987px){
    .box{
        width: 280px;
    }
    img{
        width: 280px;
    }
}
@media(max-width: 931px){
    .box{
        width: 250px;
    }
    img{
        width: 250px;
    }
}
@media(max-width: 853px){
    img{
        width: 220px;
        
    }
    .box{
        width: 250px;
    }
}
@media(max-width: 851px){
    .box{
        width: 230px;
    }
    img{
        width: 230px;
    }
}
@media(max-width: 820px){
    img{
        width: 220px;
        
    }
    .box{
        width: 250px;
    }
}
@media(max-width: 792px){
    .box{
        width: 200px;
    }
    img{
        width: 200px;
    }
}
@media(max-width: 750px)
{

    .inner-box{
        display: flex;
        justify-content: center;
        flex-direction: column;
    }
    .second, .third{
        margin-top: 20px;
    }
    img{
        padding: 20px;
        width: 400px;
    }
    .box{
        width: 440px;
    }
}
@media(max-width: 540px){
    img{
        width: 360px;
        
    }
    .box{
        width: 400px;
    }
}
@media(max-width: 463px){
    img{
        width: 270px;
        
    }
    .box{
        width: 300px;
    }
}
@media(max-width: 430px){
    img{
        width: 270px;
        
    }
    .box{
        width: 300px;
    }
}
@media(max-width: 414px){
    img{
        width: 240px;
        
    }
    .box{
        width: 270px;
    }
}
@media(max-width: 375px){
    img{
        width: 220px;
        
    }
    .box{
        width: 250px;
    }
}
@media(max-width: 360px){
    img{
        width: 200px;
        
    }
    .box{
        width: 230px;
    }
}
@media(max-width: 280px){
    img{
        width: 130px;
        
    }
    .box{
        width: 160px;
    }
}
</style>

<script setup>


</script>
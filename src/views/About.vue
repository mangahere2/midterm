<template>

    <div class="container2" id="about">

        <div class="inner-box">

            <div class="box box1">
                <img src="/images/me.jpg">
            </div>

            <div class="box box2">

                <div style="display: flex;">
                    <p class="label">Name:</p>
                    <p class="info" style="margin-left: 20px;">Levi Berdin</p>
                </div>
                
                <div style="display: flex; margin-top: 20px;">
                    <p class="label">Age:</p>
                    <p class="info" style="margin-left: 20px;">22 years old</p>
                </div>

                <div style="display: flex; margin-top: 20px; ">
                    <p class="label">Birthday:</p>
                    <p class="info"style="margin-left: 20px;">September 13, 2001</p>
                </div>

                <div style="display: flex; margin-top: 20px; ">
                    <p class="label">Address:</p>
                    <p class="info"style="margin-left: 20px;">Babag I Lapu Lapu City</p>
                </div>
                
                <div style=" margin-top: 20px; ">
                    <p class="label">"Always do your best and keep grinding"</p>
                    <p class="info"style=" margin-top: 50px; letter-spacing: 1px;">

                        My name is Levi Berdin, to be honest I am a lazy person, I make my homeworks close to
                        deadline. I almost arrive in the first subject in my schedule late, but with that out
                        of the way, I am very much motivated in grinding the things that I want to do. I do 
                        3d modelling for fun or as a hobby and I do web design for a career.
                    </p>
                </div>

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
    margin-top: 100px;
    
}
.info{
    text-align: justify;
}
img{
    width: 500px;
    height: 500px;

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
@media(max-width: 750px)
{
    .inner-box{
        display: flex;
        flex-direction: column;
    }
    .info{
    text-align: justify;
}
}

@media(max-width: 540px)
{
    img{
        width: 400px;
        height: 400px;
    }
    .info{
    text-align: justify;
}
}

@media(max-width: 430px)
{
    img{
        width: 300px;
        height: 300px;
    }
    .info{
    text-align: justify;
}
}

@media(max-width: 414px)
{
    img{
        width: 280px;
        height: 280px;
    }
    .info{
    text-align: justify;
}
}

@media(max-width: 375px)
{
    img{
        width: 250px;
        height: 250px;
    }
    .info{
    text-align: justify;
}
}

@media(max-width: 280px)
{
    img{
        width: 170px;
        height: 170px;
    }
    .info{
    text-align: justify;
}
}
</style>

<script setup>


</script>
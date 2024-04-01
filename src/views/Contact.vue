<template>

    <div class="container2" id="about">

        <div class="inner-box">

            <div class="title">
                CONTACT US
            </div>

            <div class="box">
                <div class="">
                    <input type="text" placeholder="Name" >
                </div>
                <div class="">
                    <input type="text" placeholder="Email" >
                </div>
                <div class="">
                    <input type="text" placeholder="Phone" >
                </div>
                <div class="">
                    <textarea placeholder="Message"></textarea>
                </div>

            </div>

        </div>



    </div>

</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Roboto:ital,wght@0,100;0,300;0,400;0,500;0,700;0,900;1,100;1,300;1,400;1,500;1,700;1,900&display=swap');
*{
    font-family: "Roboto", sans-serif;
    font-weight: 400;
    font-style: normal;
    letter-spacing: 2px;
}
.container2{
    min-height: 100vh;
    background: #DDDDDD;
    padding: 30px;
}
.inner-box{
    margin-top: 100px;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
}
.box{
    margin-top: 50px;
}
input, textarea{
    border: none;
    height: 47px;
    width: 600px;
    text-indent: 10px;
    margin-top: 20px;
    resize: none;
    outline: none;
}
.title{
    font-size: 45px;
}
textarea{
    height: 100px;
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
    }
}
@media(min-width: 590px){
    .container2{
        min-width: 92vw;
    }
}
@media(min-width: 569px){
    .container2{
        min-width: 92vw;
    }
}
@media(max-width: 541px){
    .container2{
        min-width: 92vw;
    }
    input, textarea{
        width: 400px;
    }
}
@media(max-width: 531px){
    .container2{
        min-width: 92vw;

    }
}
@media(max-width: 479px){
    .container2{
        min-width: 100vw;
    }
}
@media(max-width: 412px){
    .container2{
        min-width: 100vw;
        min-height: 110vh;
    }
}
@media(max-width: 375px){
    .container2{
        min-width: 100vw;
    }
    input, textarea{
        width: 250px;
    }
}
@media(max-width: 360px){
    .container2{
        min-width: 100vw;
        min-height: 120vh;
    }
    input, textarea{
        width: 250px;
    }
}
@media(max-width: 280px){
    .container2{
        min-width: 100vw;
        min-height: 120vh;
    }
    .title{
        font-size: 35px;
    }
    input, textarea{
        width: 250px;
    }
}
</style>

<script setup>


</script>
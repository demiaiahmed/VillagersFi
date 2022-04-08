<script>
    function alertMsg(){
        alert("Coming Soon Villager");
    }
</script>

<div class="header">
    <a href="https://villages.finance"><h1 class="logo">VILLAGESFI</h1></a>
    <div class="icons">
            <a class="twitter" href="https://twitter.com/villagesfi" target="_blank"><img src="img/twitter.png"></a>
            <a class="discord" href="https://discord.gg/villages" target="_blank"><img src="img/discord.png"></a>
            <a class="telegram" href="https://t.me/villagesfi" target="_blank"><img src="img/telegram.png"></a>
            <a class="medium" href="https://medium.com/@villagesfi" target="_blank"><img src="img/medium.png"></a>

    </div>
    <div class="btn">
        <a href="#">
            <img src="img/connect-wallet-button.png" alt="" on:click={alertMsg}>
        </a>
    </div>
   
</div>

<style>
*{
    margin: 0;
padding: 0;
font-family: "VT323",monospace;

}
    .header{
        height: 100px;
    width: 100%;
    background-color: black;
    background-color: rgba(0, 0, 0, 0.2);
    position: absolute;
    top: 0px;
    display: flex;
    }
    .logo{
        position: absolute;
    font-size: 50px;
    top: 20px;
    left: 30px;
    margin-right: 370px;
    color: white;
    }

    .icons a img{
        width: 50px;
    height: auto;
    }
    .icons{
        text-align: right;
        margin-right: 50px;
        flex:1;
        margin-top: 24px;
    }
    .btn{
        text-align: right;
        width:230px;
        margin-right: 20px;
        margin-top: 24px;
    }
    .btn a{
        display: block;
    }
    .btn a img{
        width: 100%;
    }

    @media only screen and (max-width:1023px){
        .logo{
            font-size: 35px;
        }
        .icons a img{
            width: 35px;
        }
    }
    @media only screen and (max-width:619px){
        .icons{
            visibility: hidden;
        }
        .btn{
            margin-left:150px;
        }
    }
@media only screen and (max-width:550px){
    .btn a img{
        width: 180px;
    }
}
</style>
<script>
    let price=0;
    function alertMsg(){
        alert("Coming Soon Villager");
    }
</script>
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="style.css">
    <link rel="shortcut icon" href="img/favicon.ico" type="image/x-icon">
    <title>VillagersFi</title>
</head>
<body>
    <div class="container">
        <div class="head">
            <div class="left-row">
                <img src="img/logo.png" class="logo" alt="">
                
                <div class="welcome">
                    <h3 style="margin-top: 1rem;">Welcome to VillagersFi!</h3>
                    <ul>
                        <li>⚔️ 10,000 Gen1 Villagers minted with $GOLD</li>
                        <li>⚔️ 5% Chance to Mint a special villager</li>
                        <li>⚔️ 5% Chance to Mint a special villager</li>
                        <li>⚔️ Stake up to 10 villagers at once in a level 1 village</li>
                    </ul>
    
                </div>
    
                <div class="two-btns">
                    <a href="#"><img src="img/villagesfi-button.png" alt="" on:click={alertMsg}></a>
                    <a href="#"><img src="img/whitepaper-button.png" alt="" on:click={alertMsg}></a>
                </div>
                <div class="docs-btn">
                    <a href="#">
                        <img src="img/docs-button.png" alt="" on:click={alertMsg}>
                    </a>
                </div>
                <div class="socials">
                    <a href="https://discord.gg/n7eyFJBw" target="_blank"><img src="img/discord.png" alt=""></a>
                    <a href="https://twitter.com" target="_blank"><img src="img/twitter.png" alt="" ></a>
                </div>
            </div>
    
            <div class="right-row">
                <div class="btn">
                    <a href="#">
                        <img src="img/connect-wallet-button.png" alt="" on:click={alertMsg}>
                    </a>
                </div>
                <div class="mintContainer">
                    <div class="mintNFT">
                        <h1>Mint Villagers</h1>
                        <div class="information">
                            <span style="font-size: 14pt;">Gen 0: 10000 / 10000</span><br>
                            <span style="font-size: 14pt;">Gen 1: ????? / 10000</span><br><br>
                            Minting Villagers Now Requires $ELIXIR<br><br>
                            You can mint up to 10 Villagers in each transaction.
                        </div>

                        <div class="formContainer">
                            <form>
                                <div class="quantityContainer">
                                    <label for="quantityText" class="quantity">
                                        Quantity:
                                    </label>
                                    <input id="quantityText" type="text" bind:value={price}>
                                </div>
                                <div>
                                    <label>
                                        <input id="quantity" type="range" class="quantitySlider"  min="0" max="10" bind:value={price}></label>
                                    </div>
                                    <div class="totalContainer">
                                        <span>Total:</span>
                                        <span class="AVAX">{price} $ELIXIR</span>
                                    </div>
                                    <div class="mintButtonContainer">
                                        <input type="image" class="mintButtonImg" name="submit" alt="Submit Form" src="img/mint_unactive_cropped.63f4d78c25b22e39b045.webp" on:click={alertMsg}>
                                    </div>
                                </form>
                        </div>
                    </div>
                </div>
    
            </div>
        </div>
        <div class="footer">
            <span>Contracts:</span>
            <div class="linkContainer">
                <a href="#" target="_blank" rel="noreferrer" on:click={alertMsg}>Villagers</a>
                <a href="#" target="_blank" rel="noreferrer" on:click={alertMsg}>Tools</a>
                <a href="#" target="_blank" rel="noreferrer" on:click={alertMsg}>Town Hall</a>
                <a href="#" target="_blank" rel="noreferrer" on:click={alertMsg}>Tower</a>
                <a href="#" target="_blank" rel="noreferrer" on:click={alertMsg}>Elixir Extractor</a>
                <a href="#" target="_blank" rel="noreferrer" on:click={alertMsg}>Walls</a>
                <a href="#" target="_blank" rel="noreferrer" on:click={alertMsg}>Canons</a>
                <a href="#" target="_blank" rel="noreferrer" on:click={alertMsg}>ELIXIR</a>
                <a href="#" target="_blank" rel="noreferrer" on:click={alertMsg}>GOLD</a>
            </div>
        </div>
    </div>
</body>



<style>
    *{

font-family: "VT323",monospace;

}
body{
background: url("img/villagesfi-background.png");

}
.container{
min-width: 370px;

}
.head{
display: flex;
flex-flow: row wrap;
justify-content: center;
width: 100%;
padding-top: 2rem;
color: #000;

}
.left-row{
display: flex;
flex-direction: column;
justify-content: center;
align-items: center;
}
.logo{
width: 14rem;
border-radius: 50%;
border: 3px solid white;
}
.welcome{
border: 4px solid #000;
border-radius: 20px;
margin-top: 1rem;
margin-left: 10pt;
margin-right: 10pt;
background-color: rgb(246, 231, 34);
padding: 5%;
display: flex;
flex-direction: column;
justify-content: center;


}
.welcome h3{
text-align: center;
display: block;
font-size:2em ;
font-weight: bold;
margin-block-start: 0.67em;
margin-block-end: 0.67em;
margin-inline-start: 0px;
margin-inline-end: 0px;
letter-spacing: 0.025em;

}
ul{
list-style: none;
}
li{
margin-bottom: 1rem;
font-size: 1.4rem;
font-weight: 300;
letter-spacing: 00.025em;
}
.two-btns{
display: flex;
justify-content: center;
margin-top: 2rem;
max-width: 100vw;
gap:1rem;
flex-wrap: wrap;
}
.two-btns a img{
height: 4rem;
}
.docs-btn{
display: flex;
justify-content: center;
margin-top: 2rem;
max-width: 100vw;
gap: 1rem;
flex-wrap: wrap;
}
.docs-btn a img{
height: 4rem;
}
.socials{
height: 4rem;
display: flex;
flex-direction: row;
justify-content: center;
margin-top: 3rem;
gap: 1rem;
}
.socials a img{
display: block;
height: 4rem;
}

.right-row{
display: flex;
flex-direction: column;
align-items: center;
justify-content: flex-start;
width: 40%;
margin-bottom: 3rem;
}
.btn{
height: auto;
display: flex;
flex-direction: row-reverse;
align-content: start;

margin-top: 1rem;
}
.btn a{
display: block;
}
.mintContainer{
width: 100%;
display: flex;
place-content: center;
margin-top: 10rem;
}
.mintNFT{
display: flex;
flex-direction: column;
justify-content: center;
align-self: center;
text-align: center;
width: 21rem;
height: 20rem;
padding-top: 4rem;
padding-bottom: 5rem;
background-image: url("img/mintbg.svg");
background-repeat: no-repeat;
background-size: cover;
background-position: center center;
}
.mintNFT h1{
margin-top: 0px;
margin-bottom: 5rem;
display: block;
font-size: 2em;
margin-block-start: 0.67em;
margin-block-end: 0.67em;
margin-inline-start: 0px;
margin-inline-end: 0px;
font-weight: bold;

}
.information{
margin-left: 13%;
margin-right:13% ;
margin-bottom: 1%;
text-align: center;
}
.formContainer{
margin-top: 0.5rem;
}
form{
display: block;
margin-top:0em ;
}
.quantityContainer{
display: flex;
flex-direction: row;
justify-content: space-between;
margin-left: 15%;
margin-right: 15%;
padding-bottom: 0.5rem;

}
label{
cursor: default;
}
#quantityText{
text-align: center;
width: 3ch;
font-family: craft;
font-size: 1.2rem;
background-color: rgb(243, 226, 170);
border-radius: 5px;
border: 1px solid black;
}
.quantitySlider {
width: 70%;
}
.totalContainer {
display: flex;
flex-direction: row;
-webkit-box-pack: justify;
justify-content: space-between;
margin-left: 15%;
margin-right: 15%;
margin-bottom: 5%;
}
.mintButtonContainer {
display: flex;
flex-direction: column;
-webkit-box-align: center;
align-items: center;
-webkit-box-pack: center;
justify-content: center;
width: 100%;
}
.mintButtonImg {
max-width: 60%;
}
.footer{
min-width: 370px;
padding-top: 20px;
padding-bottom: 20px;
display: flex;
flex-direction: column;
-webkit-box-align: center;
align-items: center;
-webkit-box-pack: center;
justify-content: center;
text-decoration: none;
font-family: craft;
color: white;
font-size: 1.2em;
}
.linkContainer {
display: flex;
-webkit-box-pack: center;
justify-content: center;
flex-wrap: wrap;
gap: 1rem;
}
.linkContainer a {
color: white;
cursor: pointer;
}

</style>
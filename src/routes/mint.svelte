
<script>
    import Header from "../components/header.svelte"
    let price=0;
    function alertMsg(){
        alert("Coming Soon Villager");
    }
</script>
    <Header />
    <div class="container">
        

        <div class="head">
            <div class="left-row">
                <h1>Pre-Sale Mint is Live!</h1>
                <div class="nft">
                    <img src="img/nft.gif" alt="">
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
            <a href="#"><img src="img/villagesfi-button.png" alt="" ></a>
            <a href="http://whitepaper.villages.finance/"><img src="img/whitepaper-button.png" alt="" ></a>
        </div>
        <div class="docs-btn">
            <a href="https://medium.com/@villagesfi">
                <img src="img/docs-button.png" alt="" >
            </a>
        </div>

    </div>




<style>
    *{

font-family: "VT323",monospace;
color: #fff;

}
:root {
    --shadow-color: #FF9E9E;
    --shadow-color-light: white;
  }
:global(body){
width: 100%;
height: 100%;
background: linear-gradient(rgba(0,0,0,0.3),rgba(0,0,0,0.3)),url(/img/background.png);
background-position: center;

}
.container{
min-width: 370px;

}
.head{
display: flex;
flex-flow: row wrap;
justify-content: center;
width: 100%;
color: #fff;
margin-bottom: 50px;
}
.left-row h1{
    color: white;
    font-size: 50px;
    font-weight: 100;
    animation: neon 3s infinite;

    text-align: center;
}
.nft{
    text-align: center;
}
.nft img{
    width: 350px;
    height: 350px;
    border-radius: 30px;
    border: solid 4px blueviolet;
}
.left-row{
display: flex;
flex-direction: column;
justify-content: center;
align-items: center;
}
.welcome{
border: 4px solid #000;
border-radius: 20px;
margin-top: 1rem;
margin-left: auto;
margin-right: auto;
background-color: #000;
padding: 25px;
display: flex;
flex-direction: column;
justify-content: center;
width:fit-content;


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
text-align: center;
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


.right-row{
display: flex;
flex-direction: column;
align-items: center;
justify-content: flex-start;
width: 40%;
margin-bottom: 3rem;
}
.btn{
position:absolute;
top: 24px;
right: 30px;
width: 230px;
}
.btn a{
display: block;
}
.btn a img{
    width: 100%;
}
.mintContainer{
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
background: #11468F;
background-repeat: no-repeat;
background-size: cover;
background-position: center center;
border: solid 2px white;
border-radius: 30px;
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

@media only screen and (max-width:1100px){
    .left-row{
        padding-top: 150px;
    }
    .head{
        flex-flow:column wrap;
    }
    .right-row{
        margin-left: auto;
        margin-right: auto;
    }
}
@keyframes neon {
    0% {
      text-shadow: -1px -1px 1px var(--shadow-color-light), -1px 1px 1px var(--shadow-color-light), 1px -1px 1px var(--shadow-color-light), 1px 1px 1px var(--shadow-color-light),
      0 0 3px var(--shadow-color-light), 0 0 10px var(--shadow-color-light), 0 0 20px var(--shadow-color-light),
      0 0 30px var(--shadow-color), 0 0 40px var(--shadow-color), 0 0 50px var(--shadow-color), 0 0 70px var(--shadow-color), 0 0 100px var(--shadow-color), 0 0 200px var(--shadow-color);
    }
    50% {
      text-shadow: -1px -1px 1px var(--shadow-color-light), -1px 1px 1px var(--shadow-color-light), 1px -1px 1px var(--shadow-color-light), 1px 1px 1px var(--shadow-color-light),
      0 0 5px var(--shadow-color-light), 0 0 15px var(--shadow-color-light), 0 0 25px var(--shadow-color-light),
      0 0 40px var(--shadow-color), 0 0 50px var(--shadow-color), 0 0 60px var(--shadow-color), 0 0 80px var(--shadow-color), 0 0 110px var(--shadow-color), 0 0 210px var(--shadow-color);
    }
    100% {
      text-shadow: -1px -1px 1px var(--shadow-color-light), -1px 1px 1px var(--shadow-color-light), 1px -1px 1px var(--shadow-color-light), 1px 1px 1px var(--shadow-color-light),
      0 0 3px var(--shadow-color-light), 0 0 10px var(--shadow-color-light), 0 0 20px var(--shadow-color-light),
      0 0 30px var(--shadow-color), 0 0 40px var(--shadow-color), 0 0 50px var(--shadow-color), 0 0 70px var(--shadow-color), 0 0 100px var(--shadow-color), 0 0 200px var(--shadow-color);
    }
  }
</style>
<script>
    import Header from "../components/header.svelte"
    let price=0;
    
</script>
    <Header />
    <div class="container">
        
        <h1 class="bigTitle">SEED ROUND IS NOW LIVE</h1>
        <div class="head">
            <div class="left-row">
                
                <div class="nft">
                    <img src="img/nft.gif" alt="">
                </div>
            </div>
    
            <div class="right-row">
                <!--<div class="btn">
                    <a href="#">
                        <img src="img/connect-wallet-button.png" alt="" on:click={alertMsg}>
                    </a>
                </div>-->
                <div class="mintContainer">
                    <div class="mintNFT">
                        <h1>SEED ROUND MINT</h1>
                        <p>⚔️ 95 Exclusive villagers with tools for sale</p>
					    <p>⚔️ Mint 10 villagers to be eligible for a free villager drop</p>
					    <p>⚔️ Each Villager will produce $ESSENCE at 5% Daily ROI</p>
					    <div class="quantityContainer">
                            <label for="quantityText" class="quantity">
                                Quantity:
                            </label>
                            <input id="quantityText" type="text" bind:value={price}>
                        </div>
					    <div class="slidebox">
						    <div>
                                <label>
                                    <input id="quantity" type="range" class="quantitySlider"  min="0" max="10" bind:value={price}></label>
                            </div>
				    	</div>
					    <div class="boxed">
					    	<a href="whitepaper.html"><img src="img/mint.png"></a>
				    	</div>
                    </div>
                </div>
                <div class="icons">
                    <a class="twitter" href="https://twitter.com/villagesfi" target="_blank"><img src="img/twitter.png"></a>
                    <a class="discord" href="https://discord.gg/villages" target="_blank"><img src="img/discord.png"></a>
                    <a class="telegram" href="https://t.me/villagesfi" target="_blank"><img src="img/telegram.png"></a>
                    <a class="medium" href="https://medium.com/@villagesfi" target="_blank"><img src="img/medium.png"></a>
        
                </div>
            </div>
        </div>
            
        

    </div>




<style>
*{
margin: 0;
padding: 0;
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
gap : 150px;
margin-top: -50px;
}
.container .bigTitle{
    margin-top: 150px;
    color: white;
    font-size: 60px;
    font-weight: 100;
	text-shadow: 0 0 1px #fff, 0 0 10px #fff, 0 0 20px #00C8FF, 0 0 30px #00C8FF, 0 0 40px #00C8FF;

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
padding-bottom: 100px;
}
.docs-btn a img{
height: 4rem;
}


.right-row{
display: flex;
flex-direction: column;
align-items: center;
justify-content: flex-start;
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
width:440px;
}
.mintNFT{
display: flex;
flex-direction: column;
justify-content: center;
align-self: center;

background-color: rgba(0, 0, 0, 0.2);
padding: 35px;
padding-bottom: 15px;
padding-top: 30px;
border-radius: 15px;
}
.mintNFT h1{
text-align: center;
margin-top: 0px;
margin-bottom: 5rem;
display: block;
font-size: 40px;
margin-block-start: 0.67em;
margin-block-end: 0.67em;
margin-inline-start: 0px;
margin-inline-end: 0px;
font-weight: bold;

}
.mintNFT p{
    font-size: 20px;
    color: white;
    margin-bottom: 10px;
}
.slidebox{
    width: 100%;
    margin-top: 20px;
    margin-bottom: 20px;
    text-align: center;
}
.slider{
    padding-top: 10px;
    padding-bottom: 30px;
}
.slide{
    width:360px;
}
.quantityContainer{
display: flex;
flex-direction: row;
justify-content: space-between;
margin-left: 0;
margin-right: 15%;
padding-bottom: 0.5rem;

}
label{
cursor: default;
}
#quantityText{
text-align: center;
color: #000;
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
.boxed{
    width: 100%;
    justify-content: center;
    align-items: center;
    align-content: center;
    text-align: center;
}
.box img{
    width: 170px;
    height: auto;
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
margin-left: 0px;
margin-right: 15%;
padding-bottom: 0.5rem;

}
label{
cursor: default;
font-size: 20px;
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
width: 85%;
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
.icons{
    visibility: hidden;
}
.icons a img{
        width: 50px;
    height: auto;
    margin-top: 24px;
    }

@media only screen and (max-width:1023px){
    .left-row{
        padding-top: 50px;
    }
    .head{
        flex-flow:column wrap;
        gap:0;
    }
    .right-row{
        margin-left: auto;
        margin-right: auto;
    }
    .right-row{
        order:-1;
    }
    .btn{
        width:200px;
        
    }
    @media only screen and (max-width:619px) {
        .icons{
            visibility: visible;
        }
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
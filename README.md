Jakub Hiža
Vianočná úloha - zvonce
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ZubZen</title>
</head>
<style>
    body{
        font-family: Jost;
    }
    header{
        display: block;
    }
    footer{
        background-color: rgb(9, 29, 62);
        color: white;
        margin-left: -8px;
        margin-right: -8px;
        margin-bottom: -50px;
        padding-left: 50px;
        padding-right: 50px;
        padding-bottom: 15px;
        padding-top: 25px;
        column-count: 4;
    }
    #hodiny{
        background-color: rgb(238, 249, 255);
        margin-left: -8px;
        margin-right: -8px;
        margin-top: -8px;
        padding-left: 50px;
        padding-bottom: 8px;
        padding-top: 8px;
        font-size: 15px;
        color: rgb(102, 100, 100);
    }
    .kontakt{
        background-color: rgb(6, 163, 218);
        color: white;
        text-align: center;
        padding-bottom: 8px;
        padding-top: 8px;
        padding-left: 30px;
        padding-right: 30px;
        margin-top: -8px;
        float: right;
    }
    #hl_ponuka{
        padding-top: 20px;
        padding-left: 20px;
        padding-right: 20px;
        padding-bottom: 20px;
    }
    .ZubZen{
        width: 200px;
        float: left;
    }
    .linky{
        text-align: right;
        font-size: 20px;
    }
    a{
        color: black;
        text-decoration: none;
        margin-left: 15px;
    }
    button{
        font-size: 20px;
        border: 0px;
        padding: 15px;
        background-color: rgb(6, 163, 218);
        color: white;
        border-radius: 5px;
    }
    #kontaktujte{
        background-color: rgb(245, 126, 96);
    }
    #starostlivost{
        position: relative;
    }
    #starostlivost img{
        width: 1857px;
        margin-left: -10px;
        margin-right: -10px;
        margin-bottom: -4px;
        position: relative;
    }
    #starostlivost button{
        margin-top: 25px;
        margin-left: 10px;
        margin-right: 10px;
    }
    .modra{
        position: absolute;
        top: 0;
        left: -8px;
        padding-right: 16px;
        width: 100%;
        height: 100%;
        background-color: rgb(9, 29, 62, 0.75);
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        color: white;
    }
    div{
        flex-direction: row;
    }
    p{
        font-size: 20px;
    }
    p img{
        width: 60px;
    }
    h3{
        font-size: 15px;
    }
    .sluzby{
        color: rgb(13, 163, 220);
        font-size: 22px;
    }
    h1{
        font-size: 45px;
        margin-top: 0px;
        margin-bottom: 0px;
    }
    #sluzby1{
        position: relative;
        top: -75px;
        color: white;
        display: flex;
        justify-content: center;
        text-align: center;
    }
    #sluzby21{
        position: relative;
        justify-content: center;
        text-align: center;
        display: flex;
        flex-direction: row;
    }
    #sluzby22{
        position: relative;
        justify-content: center;
        text-align: center;
        display: flex;
        flex-direction: row;
    }
    .div1{
        background-color: rgb(238, 249, 255);
        display: flex;
        flex-direction: column;
        position: relative;
        bottom: -250px;
        margin-left: 25px;
        margin-right: 25px;
    }
    .div1:hover{
        box-shadow: 0px 25px 25px rgb(0, 0, 0, 0.5);
    }
    .div11{
        background-color: rgb(238, 249, 255);
        display: flex;
        flex-direction: column;
        margin-left: 25px;
        margin-right: 25px;
    }
    .div11:hover{
        box-shadow: 0px 25px 25px rgba(0, 0, 0, 0.5);
    }
    .div2{
        background-color: rgb(6, 163, 218);
        color: white;
        padding-left: 50px;
        padding-right: 50px;
        margin: 15px;
        margin-bottom: 50px;
    }
    #sluzby21 h4{
        font-size: 20px;
        color: rgb(13, 163, 220);
    }
    .sluzby_male_img{
        width: 250px;
        height: 150px;
        margin: 15px;
    }
    .sluzby21img{
        width: 400px;
        margin: 15px;
    }
    .ot_hod{
        background-color: rgb(6, 163, 218);
        display: flex;
        justify-content: center;
        flex-direction: column;
        padding-left: 50px;
        padding-right: 50px;
    }
    .ot_hod button{
        background-color: white;
        color: black;
        margin: 15px;
        border-radius: 5px;
    }
    .vyhla_doktor{
        background-color: rgb(9, 29, 62);
        display: flex;
        justify-content: center;
        flex-direction: column;
        padding-left: 50px;
        padding-right: 50px;
    }
    .vyhla_doktor button{
        background-color: white;
        color: black;
        margin: 15px;
        border-radius: 5px;
    }
    .objednajtesa{
        background-color: rgb(245, 126, 96);
        display: flex;
        justify-content: center;
        flex-direction: column;
        padding-left: 50px;
        padding-right: 50px;
    }
    .objednajtesa p{
        font-size: 20px;
    }
    input{
        padding: 15px;
        margin-bottom: 10px;
        border-radius: 5px;
    }
    select{
        padding: 15px;
        border-radius: 5px;
    }
    #usetrite img{
        margin-left: -8px;
        margin-bottom: -4px;
        margin-top: 50px;
        width: 1857px;
    }
    .modra2{
        top: 2600px;
        left: 570px;
        position: absolute;
        width: 700px;
        background-color: rgb(6, 163, 218, 0.85);
        display: flex;
        flex-direction: column;
        align-items: center;
        color: white;
        padding: 30px;
        text-align: center;
    }
    #objednat{
        background-color: rgb(9, 29, 62);
    }
    #zistite{
        color: black;
        background-color: white;
    }
    #cennik{
        position: relative;
        display: flex;
        flex-direction: row;
        justify-content: center;
    }
    #cennik div{
        padding-left: 50px;
        padding-top: 75px;
        padding-bottom: 75px;
    }
    #cennik img{
        width: 300px;
    }
    #cennik p{
        color: rgb(102, 100, 100);
        font-size: 15px;
    }
    #pricebox{
        background-color: rgb(238, 249, 255);
        margin-top: -4px;
        border-bottom: 1px solid rgb(13, 163, 220);
        height: 150px;
    }
    #pricebox h4{
        font-size: 25px;
        position: relative;
        left: -27px;
        top: -125px;
    }
    #priceimg{
        margin-top: 50px;
        text-align: center;
    }
    #priceimg p{
        text-align: left;
        font-size: 20px;
        position: relative;
        top: -125px;
    }
    #priceimg button{
        position: relative;
        left: -27px;
        top: -115px;
    }
    #price€{
        background-color: rgb(238, 249, 255);
        color: rgb(13, 163, 220);
        font-size: 45px;
        position: relative;
        left: 35px;
        top: -108px;
        border-radius: 5px;
        padding: 5px;
        width: 100px;
    }
    hr{
        width: 150px;
        border-color: rgb(13, 163, 220);
    }
    #specialistii{
        margin-bottom: -175px;
    }
    #specialistivelkeimg{
        margin-left: -11px;
        margin-bottom: -4px;
        margin-top: 50px;
        width: 1860px;
    }
    #specialisti1{
        position: relative;
        display: flex;
        flex-direction: row;
        justify-content: center;
        top: -250px;
        margin-left: 500px;
        margin-right: 500px;
        margin-bottom: 50px;
    }
    #specialimg{
        width: 325px;
        height: 300px;
    }
    .special1{
        background-color: rgb(238, 249, 255);
        position: relative;
        justify-content: center;
        padding: 40px;
        margin-left: 25px;
        margin-right: 25px;
    }
    .special1 button{
        margin-top: 25px;
    }
    .special2{
        background-color: rgb(238, 249, 255);
        border: 10px white solid;
        position: relative;
        justify-content: center;
        display: flex;
        flex-direction: column;
        text-align: center;
        margin-left: 25px;
        margin-right: 25px;
    }
    .special2:hover{
        box-shadow: 0px 25px 25px rgba(0, 0, 0, 0.5);
    }
    .special3{
        background-color: rgb(238, 249, 255);
        border: 10px white solid;
        position: relative;
        justify-content: center;
        display: flex;
        flex-direction: column;
        text-align: center;
        margin-left: 25px;
        margin-right: 25px;
    }
    .special3:hover{
        box-shadow: 0px 25px 25px rgba(0, 0, 0, 0.5);
    }
    #specialisti2{
        position: relative;
        display: flex;
        flex-direction: row;
        justify-content: center;
        top: -250px;
        margin-left: 500px;
        margin-right: 500px;
        left: 17px;
    }
    .special4{
        background-color: rgb(238, 249, 255);
        border: 10px white solid;
        position: relative;
        justify-content: center;
        display: flex;
        flex-direction: column;
        text-align: center;
        margin-left: 25px;
        margin-right: 25px;
    }
    .special4:hover{
        box-shadow: 0px 25px 25px rgba(0, 0, 0, 0.5);
    }
    .special5{
        background-color: rgb(238, 249, 255);
        border: 10px white solid;
        position: relative;
        justify-content: center;
        display: flex;
        flex-direction: column;
        text-align: center;
        margin-left: 25px;
        margin-right: 25px;
    }
    .special5:hover{
        box-shadow: 0px 25px 25px rgba(0, 0, 0, 0.5);
    }
    .special6{
        background-color: rgb(238, 249, 255);
        border: 10px white solid;
        position: relative;
        justify-content: center;
        display: flex;
        flex-direction: column;
        text-align: center;
        margin-left: 25px;
        margin-right: 25px;
    }
    .special6:hover{
        box-shadow: 0px 25px 25px rgba(0, 0, 0, 0.5);
    }
    h4{
        font-size: 25px;
    }
    #kontaktimg{
        background-color: rgb(238, 249, 255);
        position: relative;
        top: -30px;
        left: 70px;
        width: 175px;
        padding: 5px;
    }
    #kontaktimg img{
        width: 35px; 
    }
    h5{
        color: rgb(13, 163, 220);
        font-size: 15px;
    }
    #scrolltop {
        display: none; 
        position: fixed; 
        bottom: 20px; 
        right: 30px; 
        z-index: 99; 
        cursor: pointer; 
        width: 50px; 
        height: 50px; 
        opacity: 0.7; 
        font-family: j;
    }
    #scrolltop:hover {
        opacity: 1; 
    }
    .hoverbutton1:hover{
        background-color: rgb(245, 126, 96);
        color: black;
    }
    .hoverbutton2{
        background-color: rgb(245, 126, 96);
    }
    .hoverbutton2:hover{
        background-color: rgb(13, 163, 220);
        color: black;
    }

</style>
<script>
    window.onscroll = function() {
    scrollFunction();
}
function scrollFunction() {
    if (document.body.scrollTop > 140 || document.documentElement.scrollTop > 140) {
        document.getElementById("scrolltop").style.display = "block";
    } else {
        document.getElementById("scrolltop").style.display = "none";
    }
}
function scrolltop() {
    document.documentElement.scrollTop = 0; 
}
</script>
<body>
    <header>
        <img src="logos/icons8-up-arrow-48.png" id="scrolltop" onclick="scrolltop()">
        <section id="hodiny">
            &#128337; Otváracie hodiny: Pon - Pia : 6.00 - 20.00
            <div class="kontakt">
                &#x2709; info@ZubZen.com &#x2706; 0911 478 254
            </div>
        </section>
        
        <section id="hl_ponuka">
            <img src="images/logo.png" class="ZubZen">
            <div class="linky">
                <strong>
                <a href="#hl_ponuka" style="color: rgb(13, 163, 220);">Úvod</a>
                <a href="#sluzby1">Služby</a>
                <a href="#cennik">Cenník</a>
                <a href="#specialistii">Naši špecialisti</a>
                </strong>
                <a><button>Objednajte sa</button></a>
            </div>
        </section>
    </header>

    <section id="starostlivost">
        <img src="images/bg-1.jpg">
        <div class="modra">
            <h3>ZUBY ZDRAVÉ, ÚSMEV KRÁSNY, STARAJTE SA O SVOJE ÚSTA KAŽDÝ DEŇ!</h3>
            <h1>Získajte najlepšiu <br> zubnú starostlivosť.</h1>
            <div>
                <a href="">
                    <button class="hoverbutton1">Objednajte sa</button>
                </a>    
                <a href="">
                    <button class="hoverbutton2">Kontaktujte nás</button>
                </a>
            </div>
        </div>
    </section>

    <section id="sluzby">
        <section id="sluzby1">
            <div class="ot_hod">
                <h2>Otváracie hodiny</h2>
                <p>Pon - Pia 6:00 - 20:00</p>
                <p>Sobota 9:00 - 16:00</p>
                <p>Nedeľa 9:00 - 13:00</p>
                <button>Objednajte sa</button>
            </div>

            <div class="vyhla_doktor">
                <h2>Vyhľadať doktora</h2>
                <input type="text" placeholder="Dátum objednania">
                <select>
                    <option>Vyberte službu</option>
                    <option>Estetická stomatológia</option>
                    <option>Zubná chirurgia</option>
                    <option>Zubé implantáty</option>
                    <option>Bielenie zubov</option>
                    
                </select>
                <a href=""><button type="reset">Vyhľadajte</button></a>
            </div>
                
            <div class="objednajtesa">
                <h2>Objednajte sa</h2>
                <p>Ak máte problémy so zubami, <br> 
                    alebo sa chcete len poradiť. <br>
                    Neváhajte nám zavolať na číslo:
                </p>
                <h1>0911 478 254</h1>
            </div>
        </section>

        <section id="sluzby21">
                <div class="nase_sluzby">
                    <img src="images/service-promo.jpg" class="sluzby21img">
                    <h3 class="sluzby">NAŠE SLUŽBY ━━ ━</h3>
                    <h1>Ponúkame iba služby tej najvyššej kvality</h1>
                </div>  

                <div class="div1">
                    <img src="images/service-1.jpg" class="sluzby_male_img">
                    <div>
                        <strong>Estetická stomatológia</strong>
                    </div>
                </div>

                <div class="div1">
                    <img src="images/service-2.jpg" class="sluzby_male_img">
                    <div>
                        <strong>Zubná chirurgia</strong>
                    </div>
                </div>
        </section>

        <section id="sluzby22">
            <div class="div11">
                <img src="images/service-3.jpg" class="sluzby_male_img">
                <div>
                    <strong>Zubé implantáty</strong>
                </div>
            </div>
            <div class="div11">
                <img src="images/service-4.jpg" class="sluzby_male_img">
                <div>
                    <strong>Bielenie zubov</strong>
                </div>
            </div>
            <div class="div2">
                <h2>Objednajte sa</h2>
                <p>Ak máte problémy so zubami, <br> 
                    alebo sa chcete len poradiť. <br>
                    Neváhajte nám zavolať na číslo:
                </p>
                <h1>0911 478 254</h1>
            </div>
        </section>
    </section>
    
    <section id="usetrite">
        <img src="images/bg-3.jpg">
        <div class="modra2">
            <h1>Ušetrite až 30% pri prvej prehliadke</h1>
            <h3>Prejdie k nám a získajte túto neskutočnú zľavu. Všetky ošetrenia a služby, súvisiace s <br>odstránením nájdených problémov počas prvej prehliadky, budú účtované so zľavou 30%</h3>
            <div>
                <a>
                    <button id="objednat">Objednajte sa</button>
                    <button id="zistite"><strong>Kontaktujte nás</strong></button>
                </a>  
            </div>
        </div>
    </section>

    <section id="cennik">
        <div>
            <h3 class="sluzby">CENNÍK━━ ━</h3>
            <h1>Ponúkame férové ceny <br> za špičkovú kvalitu</h1>
            <p>Neváhajte využiť naše príjemné a ukľudnujúce prosredie, v ktorom <br>
                sa budete cítiť bezpečne a bez zbytočných stresov.  Klinika je <br>
                vybavena najnovšími technológiami a vysoko kvalifikovaným a <br>
                profesionálnym zubným personálom, vrátane zubárov, ortodontov a <br>
                zubných hygienikov.</p>
            <h3 class="sluzby">OBJEDNAJTE SA NA ČÍSLE</h3>
            <h1>0911 478 254</h1>
        </div>

        <div id="priceimg">
            <img src="images/price/price-3.jpg">
            <div id="pricebox">
                <h1 id="price€">19€</h1>
                <h4>Dentálna hygiena <hr></h4>
                <p>Moderné zariadenie ✔</p>
                <p>Zubný Hygienik ✔</p>        
                <p>Krásny úsmev ✔</p>
                <a><button>Objednajte sa</button></a>        
            </div>
        </div>

        <div id="priceimg">
            <img src="images/price/price-1.jpg">
            <div id="pricebox">
                <h1 id="price€">35€</h1>
                <h4>Bielenie zubov <hr></h4>
                <p>Moderné vybavenie ✔</p>
                <p>Profesionálny zubár ✔</p>        
                <p>Najlepšia farba ✔</p>
                <a><button>Objednajte sa</button></a>
            </div>
        </div>
    </section>

    <section id="specialistii">
        <img src="images/bg-4.jpg" id="specialistivelkeimg">
        <div id="specialisti1">
            <div class="special1">
                <h3 class="sluzby">NAŠI ŠPECIALISTI━━ ━</h3>
                <h1>Spoznajte naších certifikovaných zubných profesionálov</h1>
                <a><button>Objednajte sa</button></a>
            </div>
            
            <div class="special2">
                <img src="images/team/team-1.jpg" id="specialimg">
                <div id="kontaktimg">
                    <img src="logos/twitter.png">
                    <img src="logos/facebok.png">
                    <img src="logos/in.png">
                    <img src="logos/instagram.png">
                </div>
                <h4>Dr. David Král</h4>
                <h5>Zubný chirurg</h5>
            </div>

            <div class="special3">
                <img src="images/team/team-2.jpg" id="specialimg">
                <div id="kontaktimg">
                    <img src="logos/twitter.png">
                    <img src="logos/facebok.png">
                    <img src="logos/in.png">
                    <img src="logos/instagram.png">
                </div>
                <h4>Dr. Katerína Králová</h4>
                <h5>Zubný chirurg</h5>
            </div>
        </div>

        <div id="specialisti2">
            <div class="special4">
                <img src="images/team/team-3.jpg" id="specialimg">
                <div id="kontaktimg">
                    <img src="logos/twitter.png">
                    <img src="logos/facebok.png">
                    <img src="logos/in.png">
                    <img src="logos/instagram.png">
                </div>
                <h4>Dr. David Král</h4>
                <h5>Zubný chirurg</h5>
            </div>

            <div class="special5">
                <img src="images/team/team-4.jpg" id="specialimg">
                <div id="kontaktimg">
                    <img src="logos/twitter.png">
                    <img src="logos/facebok.png">
                    <img src="logos/in.png">
                    <img src="logos/instagram.png">
                </div>
                <h4>Dr. David Král</h4>
                <h5>Zubný chirurg</h5>
            </div>

            <div class="special6">
                <img src="images/team/team-5.jpg" id="specialimg">
                <div id="kontaktimg">
                    <img src="logos/twitter.png">
                    <img src="logos/facebok.png">
                    <img src="logos/in.png">
                    <img src="logos/instagram.png">
                </div>
                <h4>Dr. David Král</h4>
                <h5>Zubný chirurg</h5>
            </div>
        </div>
    </section>

    <footer>
        <section class="odkazy">
           <div>
                <h2>Obľúbené odkazy</h2>
                <p>→ Úvod <br> → O nás <br> → Naši špecialisti</p>
            </div>
            <div>
                <h2>Užitočné odkazy</h2>
                <p>→ Služby <br> → Cenník <br> → Kontakt</p>
            </div>
            <div>
                <h2>Kde nás nájdete</h2>
                <p>⚲ 24 Hollého, Stará Turá, Slovensko <br> &#x2709; info@ZubZen.com <br>&#x2706; 0911 478 254</p>
            </div>
            <div>
                <h2>Sledujte nás na</h2>
                <p><img src="logos/twitter.png">
                    <img src="logos/facebok.png">
                    <img src="logos/in.png">
                    <img src="logos/instagram.png"></p>
            </div> 
        </section>
    </footer>
</body>
</html>

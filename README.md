# tehtava-5

Tehtävän koodi on jaoteltu Model-View-Controller -arkkitehtuurin mukaan. Siinä koodi on jaettu kolmeen osaan, joista jokaisella on oma roolinsa. "Model"-koodi, eli ohjelman sisältämä informaatio, "View"-koodi, joka vastaa tiedon välittämisestä käyttäjälle, sekä "Controller"-koodi, joka vastaa kahden edellä mainitun osan liittämisestä toisiinsa. 
<br/>
Product.cs edustaa tässä esimerkissä Model-koodia, eli se pitää sisällään Product-luokan ominaisuuksineen. Jokainen tuote on Product-luokan ilmentymä, jonka ominaisuuksista tuotteen tiedot noudetaan, kun niitä tarvitaan. 
<br/>
Product.cshtml taas edustaa View-koodia, eli se pitää sisällään html-koodia, joka kertoo, miten Product-luokan ominaisuudet esitetään käyttäjälle. Koodi looppaa jokaisen haetun tuotteen läpi, ja asettaa kunkin omaan "product-card"-luokan div-lohkoon. Näiden product-card -luokan elementtien ulkonäköä määritellään vielä tarkemmin site.css -tyylitiedoston ".product-card"-koodilohkossa.
<br/>
HomeController.cs -tiedosto taas edustaa controller-koodia. Tehtävänannossa mainittiin ProductController.cs, mutta sellaista ei harjoituksessa luotu, eli en osaa siitä sanoa, mutta HomeController.cs ainakin näyttää kertovan ohjelmalle, mitä tehdä, kun käyttäjä valitsee joitain navigaatiopalkin vaihtoehdoista. 
<br/>
Harjoituksessa tuotteiden hinnat eivät näkyneet, mutta kun korvasin Product.cshtml-koodissa Price-paragraafin sisällön Productin FormattedPrice-ominaisuudella, alkoivat myös hinnat näkyä.
<br/>
´´´
Eli: <p>Price: $@product.Price</p> => <p>Price: @product.FormattedPrice</p>
´´´

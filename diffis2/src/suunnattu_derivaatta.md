# Suunnattu derivaatta

# Tehtävä
> Olkoon
> \\[ f(x,y)=\frac{y^4}{x^2+1}. \\]
> Laske funktion \\( f(x, y) \\) suunnattu derivaatta ellipsin
> \\[ 2x^2+y^2=1 \\]
> ulkoyksikkönormaalin suuntaan.

[*tehtävä 1 MS-A0203 tentti 15.4.2021*](https://tenttiarkisto.fi/exams/14575/differentiaali-ja-integraalilaskenta-2/2021-04-15/)

# Esitiedot

Tehtävä vaatii kyvyn selvittää implisiittisen käyrän normaalivektorin tietyssä pisteessä. Tämä saavutetaan tutkimalla vastaavan funktion gradienttia kyseisessä pisteessä. Lisää esimerkkejä löytyy kohdasta ...

**Suunnattu derivaatta** on skalaariarvoiselle funktiolle funktio, joka kertoo, paljonko funktion arvo muuttuu liikuttaessa syöteavaruudessa tiettyyn suuntaan \\( v \\). Sen ymmärtäminen vaatii **osittaisderivaatan** määritelmän.

Suunnattu derivaatta lasketaan ottamalla pistetulo suuntavektorin ja osittaisderivaattoja sisältävän vektorin \\(\begin{bmatrix}\frac{\partial f}{\partial x}\\\\
\frac{\partial f}{\partial y} \end{bmatrix}\\) kanssa (kahden muuttujan funktio).

Tätä osittaisderivaattoja sisältävää vektoria kutsutaan funktion **gradientiksi** ja merkitään \\( \nabla f \\).

Suunnatun derivaatan arvo on luku, jonka suuruus kertoo funktion kasvunopeudesta ja etumerkki muutoksen suunnasta (kasvaako vai väheneekö funktion arvo kyseiseen suuntaan).

# Ratkaisu

Ellipsiä \\( 2x^2+y^2=1 \\) vastaava funktio on \\(  F(x, y)=2x^2+y^2-1\\), ja sen gradientti

\\( \nabla F(x, y)=\begin{bmatrix}
4x\\\\
2y
\end{bmatrix}.\\)

Ulkoyksikkönormaali tarkoittaa käyrän normaalivektoria, joka osoittaa käyrän rajaamasta alueesta poispäin ja jonka pituus on yksi.

Tarkastellaan käyrän (ellipsin) normaalivektoria pisteessä \\( (x_0, y_0) \\), jonka luonnollisesti oletetaan kuuluvan ellipsikäyrälle.

Normaalivektori saadaan sijoittamalla piste gradienttifunktioon, eli normaalivektori

\\[ \mathbf{n}= \nabla F(x_0, y_0)=\begin{bmatrix}
4x_0\\\\
2y_0
\end{bmatrix}. \\]

Normaalivektori täytyy normalisoida eli jakaa omalla pituudellaan, jolloin sen pituus on yksi.

Sen pituus on

\\[\sqrt{(4x_0)^2+(2y_0)^2}=\sqrt{4(4x_0^2+y_0^2)}=2\sqrt{4x_0^2+y_0^2}. \\]

Siispä yksikkönormaalivektori on

\\[ \hat{\mathbf{n}}=\frac{1}{2\sqrt{4x_0^2+y_0^2}}\begin{bmatrix}
4x_0\\\\
2y_0
\end{bmatrix}=\frac{1}{\sqrt{4x_0^2+y_0^2}}\begin{bmatrix}
2x_0\\\\
y_0
\end{bmatrix}. \\]

Saatu yksikkönormaali on ulkoyksikkönormaali. Tämän voi varmistaa laskemalla yksikkönormaalin jossain testipisteesdsä (kuten \\( (x_0, y_0)=(0, 1) \\)) ja argumentoimalla, että funktio on jatkuva. Vaihtoehtoisesti voi myös pohtia ellipsin yhtälöä ja sitä, miten gradientti kertoo suurimman kasvun suunnan. Tentissä perustelun ei tarvitse olla tarkka.

Funktion \\( f(x, y)=\frac{y^4}{x^2+1} \\) osittaisderivaatat ovat

\\[ \frac{\partial f}{\partial x} = -\frac{y^4}{(x^2+1)^2}\cdot 2x = -\frac{2xy^4}{(x^2+1)^2} \\]

ja

\\[ \frac{\partial f}{\partial y} = \frac{4y^3}{x^2+1}. \\]

Funktion \\( f(x, y)=\frac{y^4}{x^2+1} \\) gradientti pisteessä \\( (x_0, y_0) \\) on

\\[\nabla f(x_0, y_0)=\begin{bmatrix}
-\frac{2xy^4}{(x^2+1)^2}\\\\
\frac{4y^3}{x^2+1}
\end{bmatrix}_{\mid (x, y)=(x_0, y_0)}\\]

\\[=\begin{bmatrix}
-\frac{2x_0y_0^4}{(x_0^2+1)^2}\\\\
\frac{4y_0^3}{x_0^2+1}
\end{bmatrix}
\\]

Voidaan nyt laskea suunnattu derivaatta pisteessä \\( (x_0, y_0) \\) suuntaan \\( \hat{\mathbf{n}} \\) pistetulon avulla. Suunnattu derivaatta on

\\[f_\hat{\mathbf{n}}(x_0, y_0)= \hat{\mathbf{n}}\cdot\nabla f(x_0, y_0) \\]

\\[=\left(\frac{1}{\sqrt{4x_0^2+y_0^2}}\begin{bmatrix}
2x_0\\\\
y_0
\end{bmatrix}\right)\cdot
\begin{bmatrix}
-\frac{2x_0y_0^4}{(x_0^2+1)^2}\\\\
\frac{4y_0^3}{x_0^2+1}
\end{bmatrix}
\\]

\\[=\frac{1}{\sqrt{4x_0^2+y_0^2}}\left(\begin{bmatrix}
2x_0\\\\
y_0
\end{bmatrix}\cdot
\begin{bmatrix}
-\frac{2x_0y_0^4}{(x_0^2+1)^2}\\\\
\frac{4y_0^3}{x_0^2+1}
\end{bmatrix}\right)
\\]

\\[=\frac{1}{\sqrt{4x_0^2+y_0^2}}\left(-\frac{4x_0^2y_0^4}{(x_0^2+1)^2}+\frac{4y_0^4}{x_0^2+1}\right)
\\]

Huomaa, että kertoimen voi erottaa ulos pistetulosta.
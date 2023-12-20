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
\end{bmatrix}\\)
# HarjoitusDebuggaus
Ohjelmoinnin työkalut ja käyttäjäkokemus-kurssin tehtäviä. Avaa tehtävät klikkaamalla otsikoita. Tentti tehtävät on merkattu " [tentti]" tägillä.

Tehtävä hakemisto (https://github.com/JuusoL25/TVT26_JL/blob/main/README.md)

<details>

 <summary>  Arvaa Luku Debug </summary>
<p>
  <img width="2511" height="1404" alt="arvaa luku debuggaus" src="https://github.com/user-attachments/assets/4f979705-4f79-4946-b38e-f7bd7e7d7747" />

Screenshotin aikaisen pelin debuggaus:
1. Mikä on satunnaisesti arvottu numero? = 8
2. Kuinka monta yritystä pelaajalla menee oikean numeron arvaamiseen? = 5
3. Mikä ehto päättää pelin? = else
4. Mikä muuttuja muuttuu jokaisella kierroksella ja miten? = salainen_luku, se valikoituu aina pelin alussa rivillä 5, ja säilyy samana niin kauan kunnes pelaaja arvaa sen. Jos aloittaa uuden pelin niin muuttuja muuttuu taas välillä 1-10. 

1. Aseta breakpoint riville, jossa salainen_luku arvotaan. Selvitä mikä luku arvottiin. = 8 
2. Seuraa muuttujan yritykset arvoa jokaisella silmukan kierroksella. Kuinka monta kertaa silmukka toistuu ennen kuin peli päättyy? = 5
3. Tarkkaile muuttujan arvaus arvoa. Milloin se vastaa salainen_luku-muuttujaa? =  Arvaus arvo vastaa "salainen_luku" arvoa silloin kun se on yhtä suuri eli kun pelaaja päättelyn ja vihjeiden "liian pieni" ja "liian suuri" avulla selvittää luvun. Silloinkun pelaaja kirjoittaa arvauksen ja se on sama kun pelin alussa arvottu luku niin pelaaja voittaa.
4. Mikä ehto (if, elif, else) toteutuu kullakin kierroksella? =
Kierros yksi : if,
Kierros kaksi: if,
Kierros kolme: elif,
Kierros neljä: elif,
Kierros viisi: else,
5. Kokeile muuttaa salainen_luku kiinteäksi arvoksi (esim. salainen_luku = 7) ja tarkkaile, miten peli käyttäytyy. = Salainen luku pysyy samana jokaisella pelikerralla, eli jos pelaaja yrittää sitä uudestaan seuraavalla pelikerralla niin vastaus on sama, jolloin pelattavuus häviää = peli on kertakäyttöinen.

</p>
</details>
<br><br>

<details>
 <summary> Tenttitehtävät </summary>
 <p>
  <br><br>
<details>
<summary>  [Tentti] Word length bug debug </summary> 
<p>
<img width="2558" height="1439" alt="World lenght bug" src="https://github.com/user-attachments/assets/cf840336-7ddf-4f37-87b8-7acf6da0d771" />

Koodi käy wordlistiä läpi ja päivittää "max_length" ja "longest_word" muuttujia aina kun uusi pisin sana löytyy. Koodin rivien sisennyksen takia koodissa on ongelmia, eli tabulaattorilla koodi ensin oikein sisennetyksi. "for/if-loopissa" oli ongelma myös kohdassa "if 5>max_length". Kun koodin pitää verrata "Word length" tallennettuun max_length arvoon. Eli "5" kohdalle täytyy korvata "Word_length"
</p>
</details>

<br><br>
<details>
<summary> [Tentti] Syntax error tehtävä </summary>
<p>
<img width="2498" height="1403" alt="image" src="https://github.com/user-attachments/assets/132ac877-824b-48e5-b5d9-00c714f7169d" />

Rivillä 6 ja 7 sisennys täytyi korjata "blockin" sisään, eli "calculate_area" funktion sisään. 
Rivillä 14 "area = calculate_area(length, width" puuttui kokonaan sulkeva sulku ")". 
</p>
</details>
<br><br> 

<details>
<summary> [Tentti] Indentation error </summary>
<p>
<img width="2204" height="1274" alt="image" src="https://github.com/user-attachments/assets/56b3a905-93be-46a0-aad2-37d31bd93d86" />

Yksinkertaisesti täytyi korjata sisennys funktion sisällä, riveillä 6 ja 7
</p>
</details>
<br><br>

<details>
<summary> [Tentti] Indentation and typo error </summary>
<p>
<img width="2201" height="1345" alt="image" src="https://github.com/user-attachments/assets/936f75fe-e9d4-4a53-9130-c464f7e60909" />

Sisennysvirhe riveillä 5,6,7 ja kirjoitusvirhe rivillä 7: "len(nam)" vaikka pitäisi lukea "len(name)"
</p>

</details>
<br><br>

<details>
 <summary> [Tentti] Numerolistan sisällön purku yksittäisiin numeroihin kun kutsutaan functionia </summary>
 <p>
  <img width="2210" height="1397" alt="image" src="https://github.com/user-attachments/assets/a39e265a-e0bd-45f2-8483-b59e7612e3a1" />
  Riveillä 2,3,4 sisennys virheellinen. Korjataan se. 
  Rivillä 9 kohta "result = calculate_average(numbers)" on virheellinen, kun siitä puuttuu "*" ennen "numbers" sanaa. * symbolia käytetään kun "callataan functionia" ja halutaan purkaa listasta yksittäiset asiat. Tässä tapauksessa "result" avulla callattiin functionia "calculate_average(num1, num2, num3)". Jouduin selvittämään että miksi "*" käytetään listan sisällön purussa, koska en osannut asiaa ennestään.

 </p>
</details>
<br><br>

<details>
 <summary> [Tentti] Sisennys ja looginen virhe?  </summary>
 <p>
   <img width="2201" height="1374" alt="image" src="https://github.com/user-attachments/assets/25292cc1-08df-4b2e-84c7-8ab42174b4ae" />
   Tehtävänä oli tehdä oikeanlaiset sisennykset koodille, ja verrata odotettua "outputtia" toteutuvaan outputtiin. Tuloksena oli odotettu output eli koodissa ei ollut logiikka virhettä.

 </p>
</details>
<br><br>

<details>
 <summary> [Tentti] Laskin error tehtävä </summary>
 <p>
   <img width="2215" height="1403" alt="image" src="https://github.com/user-attachments/assets/8d514e72-f4f5-4866-9c9e-6104413be80a" />
  Sisennykset piti korjata riveillä 6,7,10,11 
   Rivillä 19 "sum_result" kutsui funktiota "multiply_numbers(a,b)" vaikka olisi pitänyt kutsua funktionia "add_numbers(a,b)" 
   Rivillä 23 "multiply_result" kutsui funktiota "add_numbers(a,b)" vaikka olisi pitänyt kutsua funktiota "multiply_numbers(a,b)"

 </p>
</details>
<br><br>
<details>
 <summary> [Tentti] Arvosana tarkistaja </summary>
 <p>
   Lähtötilanne sisennettynä:
  <img width="2208" height="1403" alt="image" src="https://github.com/user-attachments/assets/625651c6-9441-4206-a7c9-a9cd3df02a31" />

  Koodi antoi F tuloksen numeroille: 85, 75, 65, 55 koska ne eivät olleet täsmä lukuja funktiossa käytettyjen "==" symboleiden mukaisesti. Kun vaihdettiin tilalle : ">=" niin koodi antoi oikeat arvosanat. Myös rivin 20 "print" toiminto oli huonosti sisennetty.
  <img width="2212" height="1406" alt="image" src="https://github.com/user-attachments/assets/8e64db35-e797-4d68-9a67-729076486ca3" />

 </p>
</details>
<br><br> 

<details>
 <summary> [Tentti] Numerot suurempi kuin 10 </summary>
 <p>
   Lähtötilanne:
   <img width="2214" height="1399" alt="image" src="https://github.com/user-attachments/assets/2aab0026-f1c0-4e21-affc-f4b862af70a0" />
   Rivillä 6, laskennan pitäisi lähteä 0:sta eikä 1:stä. 
   Rivillä 8, on virhe ">=10" eli koodi laskee mukaan numerot jotka ovat yhtäsuuria JA isompia kuin 10. Ja koska "test_numbers" sisältää numeron 10, niin siitä tuli yksi ylimääräinen "count".

Korjattu koodi:
  <img width="2213" height="1403" alt="image" src="https://github.com/user-attachments/assets/cb30ba71-a6b6-44a3-928f-62f6ce8c8d27" />

 </p>
</details>
<br><br>

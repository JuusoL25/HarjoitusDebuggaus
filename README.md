# HarjoitusDebuggaus
Ohjelmoinnin työkalut ja käyttäjäkokemus-kurssin tehtäviä. Avaa tehtävät klikkaamalla otsikoita. Tentti tehtävät on merkattu " [tentti]" tägillä.

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

</p>
</details>



# HarjoitusDebuggaus
Debuggausharjoitusten tuloksista screenshotteja



# Arvaa Luku Debug
Screenshotin aikaisen pelin debuggaus:
1. Mikä on satunnaisesti arvottu numero? = 8
2. Kuinka monta yritystä pelaajalla menee oikean numeron arvaamiseen? = 5
3. Mikä ehto päättää pelin? = else
4. Mikä muuttuja muuttuu jokaisella kierroksella ja miten? = salainen_luku, se valikoituu aina pelin alussa rivillä 5, ja säilyy samana niin kauan kunnes pelaaja arvaa sen. Jos aloittaa uuden pelin niin muuttuja muuttuu taas välillä 1-10. 

1. Aseta breakpoint riville, jossa salainen_luku arvotaan. Selvitä mikä luku arvottiin. = 8 
2. Seuraa muuttujan yritykset arvoa jokaisella silmukan kierroksella. Kuinka monta kertaa silmukka toistuu ennen kuin peli päättyy? = 5
3. Tarkkaile muuttujan arvaus arvoa. Milloin se vastaa salainen_luku-muuttujaa? =  Arvaus arvo vastaa "salainen_luku" arvoa silloin kun se on yhtä suuri eli kun pelaaja päättelyn ja vihjeiden "liian pieni" ja "liian suuri" avulla selvittää luvun. Silloinkun pelaaja kirjoittaa arvauksen ja se on sama kun pelin alussa arvottu luku niin pelaaja voittaa.
4. Mikä ehto (if, elif, else) toteutuu kullakin kierroksella? =
Kierros yksi : if
Kierros kaksi: if
Kierros kolme: elif
Kierros neljä: elif
Kierros viisi: else
5. Kokeile muuttaa salainen_luku kiinteäksi arvoksi (esim. salainen_luku = 7) ja tarkkaile, miten peli käyttäytyy. = Salainen luku pysyy samana jokaisella pelikerralla, eli jos pelaaja yrittää sitä uudestaan seuraavalla pelikerralla niin vastaus on sama, jolloin pelattavuus häviää = peli on kertakäyttöinen.


#Word lenght bug debug
Koodi käy wordlistiä läpi ja päivittää "max_lenght" ja "longest_word" muuttujia aina kun uusi pisin sana löytyy. Koodin rivien sisennyksen takia koodissa on ongelmia, eli tabulaattorilla koodi ensin oikein sisennetyksi. "for/if-loopissa" oli ongelma myös kohdassa "if 5>max_lenght". Kun koodin pitää verrata "Word length" tallennettuun max_lenght arvoon. Eli "5" kohdalle täytyy korvata "Word_lenght"


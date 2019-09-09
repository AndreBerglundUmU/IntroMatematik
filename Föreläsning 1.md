# Föreläsning 1
Innehåller:
1. Mängdlära
   - Användbara mängder
   - Mängdoperationer
2. Logik
   - Konnektiv och kvantifikatorer
   - Sanningsvärdestabeller
   
   
Det är lite besvärligt att definiera koncept som är så grundläggande som dessa, så vi kommer att nöja oss med att säga att **mängder** är samlingar av **element**. Vi använder klamrar, ![equation](https://latex.codecogs.com/gif.latex?%5C%7B%5Cldots%5C%7D),
för att gruppera vilka element som är inkluderade i mängden. 

Exempel: 

![equation](https://latex.codecogs.com/gif.latex?%5C%7B%5Ctext%7Bgul%7D%2C%5Ctext%7Bvit%7D%2C%5Ctext%7Borange%7D%5C%7D)

![equation](https://latex.codecogs.com/gif.latex?%5C%7B2%2C3%2C5%2C7%2C11%5C%7D)


En speciell mängd är den tomma mängden, som definieras enligt:
![equation](https://latex.codecogs.com/gif.latex?%5Cemptyset%20%3A%3D%20%5C%7B%5C%7D)
Notera också användandet av ":=" vilket indikerar att vi från och med nu har definierat det att mena det på höger sida. Ett intressant faktum är att det är ett av sätten att börja definiera de naturliga talen. 
Vi ser ganska naturligt att det finns 0 element i den tomma mängden, så vi skriver det som
![equation](https://latex.codecogs.com/gif.latex?%7C%5Cemptyset%7C%20%3D%200).

En notation som är viktig är hur man beskriver att ett element ligger i en mängd eller ej. Detta görs med hjälp av tecknen
![equation](https://latex.codecogs.com/gif.latex?%5Cin) och 
![equation](https://latex.codecogs.com/gif.latex?%5Cnotin).

Exempel: Om vi definierar mängden
![equation](https://latex.codecogs.com/gif.latex?A%20%3D%20%5C%7B1%2C2%2C3%5C%7D)
så kan vi skriva att 
![equation](https://latex.codecogs.com/gif.latex?1%5Cin%20A)
och motsvarande, att 
![equation](https://latex.codecogs.com/gif.latex?5%5Cnotin%20A). Naturligtvis så ser vi också att 
![equation](https://latex.codecogs.com/gif.latex?%7CA%7C%20%3D%203).

Med hjälp av den notationen kan vi använda kriterier för att begränsa vilka element som är inkluderade i mängden med hjälp av ":".

Exempel: Om vi definierar mängden 
![equation](https://latex.codecogs.com/gif.latex?%5COmega%20%3D%20%5C%7B1%2C2%2C3%2C4%2C5%2C6%2C7%2C8%2C9%5C%7D)
, så kan vi skriva
![equation](https://latex.codecogs.com/gif.latex?A%20%3D%20%5C%7B2%2C4%2C6%2C8%5C%7D%20%3D%20%22%5Ctext%7BAlla%20j%7B%5C%22a%7Dmna%20tal%20i%20%7D%20%5COmega%22%20%3D%20%5C%7Bx%5Cin%5COmega%20%3A%202%7Cx%5C%7D).

## Användbara mängder
Nedan följer mängder som ni förväntas kunna och använda er av.

![equation](https://latex.codecogs.com/gif.latex?%5Cmathbb%7BN%7D%20%3D%20%5Ctext%7B%22De%20naturliga%20talen%22%7D%20%3D%20%7B1%2C2%2C3%2C4%2C%5Cldots%7D)

![equation](https://latex.codecogs.com/gif.latex?%5Cmathbb%7BZ%7D%20%3D%20%5Ctext%7B%22Heltalen%22%7D%20%3D%20%7B%5Cldots%2C-4%2C-3%2C-2%2C-1%2C0%2C1%2C2%2C3%2C4%2C%5Cldots%7D)

![equation](https://latex.codecogs.com/gif.latex?%5Cmathbb%7BQ%7D%20%3D%20%5Ctext%7B%22De%20rationella%20talen%22%7D%20%3D%20%5Cleft%5C%7B%20x%3A%20x%20%3D%20%5Cfrac%7Ba%7D%7Bb%7D%2C%20a%5Cin%5Cmathbb%7BZ%7D%2C%20b%5Cin%5Cmathbb%7BZ%7D%5Csetminus%5C%7B0%5C%7D%5Cright%5C%7D)

![equation](https://latex.codecogs.com/gif.latex?%5Cmathbb%7BR%7D%20%3D%20%5Ctext%7B%22De%20reella%20talen%22%7D)

![equation](https://latex.codecogs.com/gif.latex?%5Cmathbb%7BC%7D%20%3D%20%5Ctext%7B%22De%20komplexa%20talen%22%7D%20%3D%20%5C%7Bz%3A%20z%20%3D%20a&plus;bi%2C%20%5Cquad%20a%2Cb%5Cin%5Cmathbb%7BR%7D%5C%7D)

Det kan vara bra att veta att alla dessa mängder är i direkt relation med varandra, elementen från den första finns i den andra, elementen i den andra finns i den tredje, osv.. Det går att skriva som:

![equation](https://latex.codecogs.com/gif.latex?%5Cmathbb%7BN%7D%20%5Csubset%20%5Cmathbb%7BZ%7D%20%5Csubset%20%5Cmathbb%7BQ%7D%20%5Csubset%20%5Cmathbb%7BR%7D%20%5Csubset%20%5Cmathbb%7BC%7D)

Och med det ger vi följande definition:

**Definition:** Delmängd och äkta delmängd.
Vi säger att en mängd B är en **delmängd av A** om alla element i B också ligger i A. Det skrivs
![equation](https://latex.codecogs.com/gif.latex?B%5Csubseteq%20A).
Om 
![equation](https://latex.codecogs.com/gif.latex?B%5Csubseteq%20A)
och
![equation](https://latex.codecogs.com/gif.latex?B%5Cneq%20A)
så är B en **äkta delmängd av A**. Det skrivs 
![equation](https://latex.codecogs.com/gif.latex?B%5Csubset%20A).

## Mängdoperationer
Nu när vi har de grundläggande sätten att konstruera mängder, så kan vi definiera hur man kan applicera olika typer av funktioner på dem. 

![equation]()
![equation]()
![equation]()
![equation]()
![equation]()
https://www.codecogs.com/latex/eqneditor.php

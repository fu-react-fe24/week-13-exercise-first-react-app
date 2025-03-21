# Vecka 13: My First React App

I den här övningen är tanken att du skall få en "steg-för-steg"-guide i hur du går till väga för att skapa upp ditt första React-projekt, samt använda några av de mest grundläggande teknikerna och tankesätten.
Tills detta satt sig i autopiloten så kan ni använda vissa av stegen i denna övning som en lathund till att skapa era nya React-appar under kommande veckor.

## **Steg 1:** Ladda hem och installera Node.js

För att kunna skapa upp våra React-appar måste vi först ladda ner Node.js, som hjälper oss med vår pakethantering via npm (node package manager), samt att kunna köra utvecklingsverktyg som Vite. Nedladdening för Node.js [hittar du här](https://nodejs.org). Klickar ni på *Download Node.js (LTS)* så får ni automatiskt ner den versionen av Node som passar ert operativsystem. Ni kan också klicka på *Download* i menyn för att anpassa den version ni vill ladda ner, men jag skulle verkligen rekommendera att ni väljer **LTS** och inte **Current**. Detta då LTS står för *Long Time Support* och oftast är mer stabila.

När ni laddat hem Node så installerar ni det genom att öppna installationsfilen. Ändra inga inställningar (om ni inte vet vad ni gör) utan klicka er bara fram till installationen och kör igång den.

För att testa att allt gått rätt till så kan ni öppna valfri terminal och köra kommandot nedan för att få upp den version av Node som ni nu har installerat på era datorer.

```
node -v
```

I skrivande stund är den senaste LTS-versionen 22.14.0. Har ni en äldre version redan installerade så kan ni följa detta steg från start för att få den senaste versionen.

## **Steg 2:** NPM och Vite

Nästa steg är att se till så att vi har korrekt version av npm (node package manager), samt att installera Vite. Börja med att köra följande kommando i valfri terminal:

```
npm -v
```

Detta bör resultera i att du får upp den version av npm som automatiskt skall ha följt med vid installationen av Node. Får du inte upp ett versionsnummer så har någonting gått snett, och du behöver antagligen installera om Node på nytt. Den senaste versionen av npm är i skrivande stund 11.2.0. Får du upp en äldre version så kan du uppdatera genom att köra kommandot nedan:

```
npm i -g npm
```

Testa sedan om det fungerade genom att återigen köra kommandot för version ovan.

När vi nu har npm "up and running" så kan vi äntligen installera Vite. Detta gör du genom att köra nedanstående kommando:

```
npm i -g vite
```

Kontrollera din installation genom att köra:

```
vite -v
```

Senaste versionen är i skrivande stund 6.2.2.

## **Steg 3:** Skapa din React-app

Öppna nu valfri terminal (**INTE** Git Bash) i den mapp på datorn där du vill skapa din React-app. Tidigare i denna guide spelade det igen roll var du öppnade terminalen, men nu är det viktigt att du står i den mapp där ditt projekt skall hamna. Kör kommandot nedan för att skapa upp din React-app med byggverktygen Vite.

```
npm create vite@latest
```

Detta går jättesnabbt och du kommer få tipset om att köra följande kommandon i tur och ordning:

```
cd [namnet-på-projektet]
npm install
npm run dev
```

Jag skulle dock vilja tipsa er om att smyga in ett ```code .``` innan du kör ```npm run dev``` eftersom det sistnämnda kommer uppehålla terminalen med din utvecklingsserver. Om du öppnar längen för din utvecklingsserver som dyker upp i terminalen (oftast localhost:5173) så kommer öppnas din app i webbläsaren. Från och med nu så gör vi såhär istället för att klicka på "Go Live" i VS Code vilket inte kommer att fungera på React-applikationer. 

# Connected ADO.NET: De Mol

De spelers van De Mol moeten hun status in het spel kunnen opzoeken via
een

applicatie waarmee ze kunnen achterhalen of ze de mol zijn. Verder
kunnen ze in

een profielvenster zien wanneer en waar hun spel verloopt.

MainWindow

![](./media/image1.png)

ProfileWindow voor een speler

![Afbeelding met tekst, beeldscherm, mobiele telefoon, scherm
Automatisch gegenereerde beschrijving](./media/image2.png)

ProfileWindow voor de mol

![Afbeelding met tekst Automatisch gegenereerde
beschrijving](./media/image3.png)

Gebruik het sql script, "mollenscript.sql" om de tabel spelers en
spellen aan te

maken en te vullen met data.

1.  Als speler kan ik de invoervelden voor naam en wachtwoord gebruiken
    om mee in te loggen. Indien er één of meer regels in de database
    zitten die dezelfde naam en hetzelfde wachtwoord hebben, dan wordt
    ik ingelogd.

2.  Als een speler wordt ingelogd, dan wordt het profielvenster getoond
    met de informatie van de ingelogde speler.

3.  Afhankelijk van de status van de speler wordt de tekst in de
    respectievelijke kleur getoond in het profielvenster.

// De mol kleur : #e0371d

> // De niet mol kleur : #61f1f1

4.  Afhankelijk van de status van de ingelogde speler wordt de
    afbeelding aangepast:

    a.  De mol ziet de afbeelding: "DeMolRed.jpg"

    b.  De niet-mollen zien de afbeelding: "DeMol.jpg"

5.  Als gebruiker kan ik de checkbox SQL injectie activeren.

    a.  Als de checkbox is uitgevinkt, maakt het programma achterliggend
        gebruik van SqlParameter's om de naam en wachtwoord van een
        speler door te geven aan het SqlCommand.

    b.  Als de checkbox is aangevinkt, maakt het programma achterliggend
        gebruik van string interpolatie om de naam en wachtwoord van een
        speler door te geven aan het SqlCommand.

Tips:

1.  Maak gebruik van een methode ZetKleur(Color kleur) die de tekst in
    het profielvenster van kleur verandert.

2.  Maak gebruik van een methode GetSpel die het spel van de speler
    ophaalt uit de database.

3.  Het aanpassen van een imagesource doe je m.b.v. een BitmapImage en
    een Uri.

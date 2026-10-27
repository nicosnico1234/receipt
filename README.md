# Kvittering

Statisk side, der viser en digital kvittering fra et NFC-tap. Del af et bachelorprojekt på DTU om digital kvitteringslevering ved kassen.

Hele kvitteringen står komprimeret i linkets `#`-del: `https://nicosnico1234.github.io/receipt/#r1.<base64url(raw deflate(JSON))>`. Browseren sender aldrig `#`-delen til serveren, så GitHub ser ikke kvitteringerne, kun at siden blev hentet.

Siden gemmer viste kvitteringer i browserens lager på telefonen ("Mine kvitteringer"). Intet sendes videre.

Siden må ikke indeholde analyse- eller sporingsscripts, fordi de kan læse hele adressen og de gemte kvitteringer.

Kildekoden vedligeholdes i et privat repo og kopieres hertil. Ret ikke i filerne her direkte.

Prototype: kvitteringerne er fra et simuleret kassesystem og er ikke signeret endnu.

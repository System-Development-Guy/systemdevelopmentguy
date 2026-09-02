# Indhold

[[#Hvorfor bruge markdown filer og format?]]

[[#Markdown]]

[[#Grundlæggende Syntaks]]

[[#Heading]]

[[#H1]]

[[#H2]]

[[#H3]]

[[#H4]]

[[#H5]]

[[#Bold]]

[[#Italic]]

[[#Blockquote]]

[[#Ordered List]]

[[#Unordered List]]

[[#Code]]

[[#Horizontal Rule]]

[[#Link]]

[[#Image]]

[[#Udvidet Syntaks]]

[[#Table]]

[[#Fenced Code Block]]

[[#Footnote]]

[[#Heading ID]]

[[#My Great Heading { custom-id}]]

[[#Definition List]]

[[#Strikethrough]]

[[#Task List]]

[[#Emoji]]

[[#Highlight]]

[[#Subscript]]

[[#Superscript]]

[[#Highlight text]]

[[#Lidt historie]]

[[#Fjernskriver (Telex)]]

[[#ITA-2 encoding]]

[[#ASCII kontrol karakterer (kode 0-31)]]

[[#ASCII udskrivbare karakterer (kode 32-127)]]

[[#Det udvidede ASCII tegnsæt  (Kode 128-255)]]

[[#Præsentation]]

[[#Kildehenvisninger]]

Opdateret 2026AUG05 2.0.0

<div style="page-break-after: always; visibility: hidden">\pagebreak\</div>

# Hvorfor bruge markdown filer og format?
[[#Indhold]]
Dette dokument giver en generel introduktion til, hvad Markdown-filer er, og hvordan Markdown anvendes.

Dokumentet er ikke udtømmende. Det er under løbende udvikling og vil blive udformet, så I kan bruge det som opslagsværk.

# Markdown
[[#Indhold]]

Markdown er et letvægts-markupformat, der gør det muligt at tilføje struktur og enkel formatering til almindelig tekst.

En væsentlig idé bag Markdown er, at dokumentet fortsat skal være forholdsvis let at læse, selv når man ser den rå Markdown-kilde.

Markdown blev introduceret af John Gruber i 2004.

Markdown-syntaks kan overordnet opdeles i:

1. grundlæggende syntaks
2. udvidet syntaks

Det er vigtigt at være opmærksom på, at der findes forskellige **Markdown-varianter** og renderere. Derfor fungerer ikke al syntaks nødvendigvis ens i eksempelvis:

- Obsidian
- Visual Studio Code
- GitHub
- GitLab
- forskellige Markdown-preview-plugins

## Grundlæggende Syntaks
[[#Indhold]]

Følgende elementer understøttes af de fleste Markdown-renderere.
Benævnelserne er ofte på engelsk.

# Heading
[[#Indhold]]

# H1
[[#Indhold]]

## H2
[[#Indhold]]

### H3
[[#Indhold]]

#### H4
[[#Indhold]]

##### H5
[[#Indhold]]

### Bold
[[#Indhold]]

**bold text**

### Italic
[[#Indhold]]

*italicized text*

### Blockquote (til citater)
[[#Indhold]]

> blockquote

### Nummereret Liste
[[#Indhold]]

1. Første element
2. Andet element
3. Tredje element

### Unummereret Liste
[[#Indhold]]

- Første element
- Andet element
- Tredje element

### Kode linje
[[#Indhold]]

`code`

### Horizontal Rule
[[#Indhold]]

---

### Link
[[#Indhold]]

[Markdown Guide](https://www.markdownguide.org)

### Billeder
[[#Indhold]]

`![Morsetaste](./Attachments/Morsetaste.jpg)`

![Morsetaste](./Attachments/Morsetaste.jpg)

Skaleret billede (obsidan)

`![[Morsetaste.jpg|300]]`

![[Morsetaste.jpg|300]]

Skaleret billede (Visual Studio Code)
Kræver plugin 

https://marketplace.visualstudio.com/items?itemName=bierner.markdown-image-size

Denne syntaks er **ikke standard-Markdown** og fungerer derfor ikke nødvendigvis i andre Markdown-renderere.

#### Skalering i Visual Studio Code

Muligheden afhænger af den valgte Markdown-renderer eller installerede udvidelser.

Eksempel på udvidelse:

[https://marketplace.visualstudio.com/items?itemName=bierner.markdown-image-size](https://marketplace.visualstudio.com/items?itemName=bierner.markdown-image-size)

En renderer eller udvidelse kan eksempelvis understøtte:

`![](./Attachments/Morsetaste.jpg =250x)`

Dette er ikke en del af den grundlæggende Markdown-standard.

![](./Attachments/Morsetaste.jpg =250x)

## Udvidet Syntaks

Udvidet Markdown-syntaks giver flere muligheder end den grundlæggende syntaks.

Det er vigtigt at være opmærksom på, at ikke alle Markdown-editorer og renderere understøtter de samme udvidelser.

### Tabel
[[#Indhold]]

| Syntax    | Description |
| --------- | ----------- |
| Header    | Title       |
| Paragraph | Text        |

### Afgrænset kodeblok – Fenced Code Block
[[#Indhold]]

```json
{
  "firstName": "John",
  "lastName": "Smith",
  "age": 25
}
```

Det er en fordel at angive programmeringssproget (i dette tilfælde `JSON`) efter de tre backticks, hvis rendereren understøtter syntax highlighting.

### Fodnote
[[#Indhold]]

Here's a sentence with a footnote. [^1]

[^1]: This is the footnote.

### Heading ID
[[#Indhold]]

Nogle Markdown-renderere understøtter eksplicitte ID'er på overskrifter:

### My Great Heading {#custom-id}
[[#Indhold]]

Dette er ikke universelt understøttet.
### Definitionsliste – Definition List
[[#Indhold]]

term
: definition

### Gennemstreget – Strikethrough
[[#Indhold]]

~~The world is flat.~~

### Opgave liste
[[#Indhold]]

- [x] Write the press release
- [ ] Update the website
- [ ] Contact the media

### Emoji
[[#Indhold]]

That's so funny! 😂

### Fremhævning i Obsidian
[[#Indhold]]

I need to highlight these ==very important words==.

### Fremhævning i Visual Studio Code
[[#Indhold]]

Visual Studio Code kan kræve en udvidelse for at fortolke samme syntaks som fremhævning.

Eksempel:

https://marketplace.visualstudio.com/items?itemName=DaCodeKid.vscode-mark-highlighter

I need to highlight these ==very important words==.

### Sænket skrift
[[#Indhold]]

Markdown understøtter ikke nødvendigvis subscript direkte, men mange renderere tillader HTML:

`H<sub>2</sub>O` og kan så præsenteres som H<sub>2</sub>O.

### Hævet skrift
[[#Indhold]]

s<sup>uperman</sup>

# Markeret tekst
Nogle Markdown-renderere tillader HTML direkte i dokumentet.

Eksempel: <span style="background-color: #FFFF00">Marked text</span> eller <span style="background-color: #FF0000"><font color="#FFFFFF">Marked text</font></span>.

<div style="page-break-after: always; visibility: hidden">\pagebreak\</div>

## Lidt historie
[[#Indhold]]

Udveksling af information elektronisk er ikke så enkelt, som man umiddelbart skulle tro.

Et vigtigt skridt mod standardiseret elektronisk kommunikation blev taget med udviklingen af den elektriske telegraf og morsekoden i 1800-tallet. I 1844 demonstrerede Samuel Morse og Alfred Vail en telegrafforbindelse mellem Washington D.C. og Baltimore.

For at sende information blev der anvendt en telegraf.

![Telegrafo](./Attachments/Telegrafo.png)

Telegraf – Wikipedia

Telegrafen fungerer ved, at et elektrisk kredsløb sluttes, når telegraftasten trykkes ned. Dermed løber der strøm gennem en elektromagnet.

Strømmen gennem spolens viklinger skaber et magnetfelt, som kan påvirke en mekanisk del i modtageren. På de tidlige registrerende telegrafer kunne denne bevægelse bruges til at lave mærker på en papirstrimmel.

Da papirstrimlen blev fremført med en konstant hastighed, kunne længden af signalerne registreres som henholdsvis korte og lange signaler.

[Video om telegraf](https://www.youtube.com/shorts/9DCP4TMYg_M)

Som det ses af illustrationerne herunder, var tidsintervallet mellem signalerne en vigtig del af den amerikanske morsekode.

Den internationale morsekode standardiserede senere forholdet mellem signalernes længder. En prik (_dit_) udgør én tidsenhed, mens en streg (_dah_) udgør tre tidsenheder. Mellemrummene mellem signaler, bogstaver og ord defineres ligeledes i tidsenheder.


| Amerikansk morse kode (1844)                                                            | International morse kode (1865)                                                                            |
| --------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------- |
| ![American](./Attachments/American_Morse_Code_-_letters.svg.png)                        | ![international](./Attachments/InternationalMorseWithNumbers.PNG)                                          |
| ![Amercode](./Attachments/Amercode.png)                                                 |                                                                                                            |
| Morsetempo:<br><br>Den Amerikanske morse kode inde-<br>holdte mellemrum (ophold i tid). | Morsetempo (enhed):<br><br>1. Længden af en prik er en enhed (unit).<br>2. En streg svarer til tre enheder |
Kilde: wikipedia

Morsekoderne tog primært udgangspunkt i det latinske alfabet, og derfor opstod der behov for at repræsentere yderligere nationale tegn.

I Danmark anvender vi eksempelvis bogstaverne `æ`, `ø` og `å`. I forskellige kommunikationssystemer har sådanne tegn derfor enten fået egne repræsentationer eller været omskrevet, eksempelvis som `ae`, `oe` og `aa`.

Andre lande stod over for tilsvarende problemer.

Dette illustrerer et grundlæggende problem, som fortsat er relevant i moderne IT: **Hvordan sikrer vi, at afsender og modtager fortolker de samme bit som de samme tegn?**

Det er netop dette problem, som tegnkodninger forsøger at løse.

## Fjernskriver (Telex)
[[#Indhold]]

[Video om telex skriver](https://youtu.be/KrzJqC_RtSU?t=50)

Telex blev udviklet med udgangspunkt i teleprinterteknologi. Udviklingen af det automatiske telexsystem begyndte i Tyskland i 1920'erne, og en offentlig telexservice blev sat i drift i 1933.

En væsentlig fordel ved systemet var, at en besked kunne forberedes på forhånd på en perforeret papirstrimmel. Maskinen kunne derefter læse strimlen og transmittere beskeden automatisk.

Traditionel telexkommunikation fungerede typisk med en signalhastighed på **50 baud**, hvilket svarede til omtrent **66 ord pr. minut**.

Det optimerede anvendelsen af forbindelsen, fordi operatøren ikke behøvede at skrive hele beskeden manuelt, mens forbindelsen var optaget.

Tankegangen er stadig relevant i moderne datakommunikation: transmissionskapacitet er en begrænset ressource, og vi ønsker derfor at udnytte forbindelser og båndbredde så effektivt som muligt.

## ITA-2 encoding
[[#Indhold]]

[Video om telex skriver - giver Bell (klokke) signal](https://www.youtube.com/shorts/C2GdPW10leE)

ITA2 står for **International Telegraph Alphabet No. 2**.

ITA2 anvender en **5-bit-kode**, hvilket giver: $2^5 = 32$ mulige bitkombinationer.

32 kombinationer er ikke nok til både alfabetet, cifre, tegn og kontrolfunktioner. Derfor anvender ITA2 to tilstande:

- `LTRS` – Letters
- `FIGS` – Figures

Den samme bitkombination kan dermed have forskellig betydning afhængigt af, om systemet befinder sig i Letters- eller Figures-tilstand.

| **Dec** | **Ltr** | **Fig** | **Hex** | **Bin** | **Remark**                        |
| ------- | ------- | ------- | ------- | ------- | --------------------------------- |
| 0       | NUL     |         | 00      | 000·00  | NULL, Nothing (blank tape)        |
| 1       | E       | 3       | 01      | 000·01  |                                   |
| 2       | LF      |         | 02      | 000·10  | Line Feed (new line)              |
| 3       | A       | -       | 03      | 000·11  |                                   |
| 4       | SP      |         | 04      | 001·00  | Space                             |
| 5       | S       | '       | 05      | 001·01  |                                   |
| 6       | I       | 8       | 06      | 001·10  |                                   |
| 7       | U       | 7       | 07      | 001·11  |                                   |
| 8       | CR      |         | 08      | 010·00  | Carriage Return                   |
| 9       | D       | ENC     | 09      | 010·01  | Enquiry (Who are you?, WRU)       |
| 10      | R       | 4       | 0A      | 010·10  |                                   |
| 11      | J       | BEL     | 0B      | 010·11  | BELL (ring bell at the other end) |
| 12      | N       | ,       | 0C      | 011·00  |                                   |
| 13      | F       | !       | 0D      | 011·01  | Can also be %                     |
| 14      | C       | :       | 0E      | 011·10  |                                   |
| 15      | K       | (       | 0F      | 011·11  |                                   |
| 16      | T       | 5       | 10      | 100·00  |                                   |
| 17      | Z       | **+**   | 11      | 100·01  |                                   |
| 18      | L       | )       | 12      | 100·10  |                                   |
| 19      | W       | 2       | 13      | 100·11  |                                   |
| 20      | H       | $       | 14      | 101·00  | Currency symbol — Can also be £   |
| 21      | Y       | 6       | 15      | 101·01  |                                   |
| 22      | P       | 0       | 16      | 101·10  |                                   |
| 23      | Q       | 1       | 17      | 101·11  |                                   |
| 24      | O       | 9       | 18      | 110·00  |                                   |
| 25      | B       | ?       | 19      | 110·01  |                                   |
| 26      | G       | &       | 1A      | 110·10  | Can also be @                     |
| 27      | FIGS    |         | 1B      | 110·11  | Figures (Shift on)                |
| 28      | M       | .       | 1C      | 111·00  |                                   |
| 29      | X       | /       | 1D      | 111·01  |                                   |
| 30      | V       | ;       | 1E      | 111·10  |                                   |
| 31      | LTRS    |         | 1F      | 111·11  | Letters (Shift off)               |

![baudot](./Attachments/baudot.svg)

Kilde: Cryptomuseum.com

ITA2 er et godt eksempel på en tidlig tegnkodning, hvor et bestemt bitmønster repræsenterer et tegn eller en kontrolfunktion.

Senere opstod behovet for en tegnkodning med plads til flere tegn og kontrolfunktioner. En vigtig standard blev **ASCII**, som står for **American Standard Code for Information Interchange**.

ASCII er oprindeligt en **7-bit-tegnkodning**. 

Med 7 bit kan der dannes: $2^7 = 128$ forskellige bitkombinationer.

ASCII indeholder derfor koder fra **0 til 127**.

## ASCII kontrol karakterer (kode 0-31 og 127)
[[#Indhold]]

ASCII indeholder en række kontroltegn, som oprindeligt blev anvendt til blandt andet terminaler, teleprintere og kommunikationsudstyr.

Koderne **0–31** er kontroltegn.

Eksempler er:

- `NUL` – Null
- `BEL` – Bell
- `BS` – Backspace
- `LF` – Line Feed
- `CR` – Carriage Return
- `ESC` – Escape

Desuden er kode **127**, `DEL` (_Delete_), også et kontroltegn.

Bemærk, at ASCII er en 7-bit-kodning. Hvis binære værdier i tabellen vises med otte cifre, eksempelvis `01000001`, er det blot ASCII-værdien med et ekstra indledende `0`.

| DEC | OCT | HEX | BIN         | Symbol | HTML Number | HTML Name | Description                 |
| --- | --- | --- | ----------- | ------ | ----------- | --------- | --------------------------- |
| 0   | 000 | 00  | 0000000     | NUL    | &#00;       |           | Null character              |
| 1   | 001 | 01  | 0000001     | SOH    | &#01;       |           | Start of Heading            |
| 2   | 002 | 02  | 0000010     | STX    | &#02;       |           | Start of Text               |
| 3   | 003 | 03  | 0000011     | ETX    | &#03;       |           | End of Text                 |
| 4   | 004 | 04  | 0000100     | EOT    | &#04;       |           | End of Transmission         |
| 5   | 005 | 05  | 0000101     | ENQ    | &#05;       |           | Enquiry                     |
| 6   | 006 | 06  | 0000110     | ACK    | &#06;       |           | Acknowledge                 |
| 7   | 007 | 07  | 0000111     | BEL    | &#07;       |           | Bell, Alert                 |
| 8   | 010 | 08  | 0001000     | BS     | &#08;       |           | Backspace                   |
| 9   | 011 | 09  | 0001001     | HT     | &#09;       |           | Horizontal Tab              |
| 10  | 012 | 0A  | 0001010     | LF     | &#10;       |           | Line Feed                   |
| 11  | 013 | 0B  | 0001011     | VT     | &#11;       |           | Vertical Tabulation         |
| 12  | 014 | 0C  | 0001100     | FF     | &#12;       |           | Form Feed                   |
| 13  | 015 | 0D  | 0001101     | CR     | &#13;       |           | Carriage Return             |
| 14  | 016 | 0E  | 0001110     | SO     | &#14;       |           | Shift Out                   |
| 15  | 017 | 0F  | 0001111     | SI     | &#15;       |           | Shift In                    |
| 16  | 020 | 10  | 0010000     | DLE    | &#16;       |           | Data Link Escape            |
| 17  | 021 | 11  | 0010001     | DC1    | &#17;       |           | Device Control One (XON)    |
| 18  | 022 | 12  | 0010010     | DC2    | &#18;       |           | Device Control Two          |
| 19  | 023 | 13  | 0010011     | DC3    | &#19;       |           | Device Control Three (XOFF) |
| 20  | 024 | 14  | 0010100     | DC4    | &#20;       |           | Device Control Four         |
| 21  | 025 | 15  | 0010101     | NAK    | &#21;       |           | Negative Acknowledge        |
| 22  | 026 | 16  | 0010110     | SYN    | &#22;       |           | Synchronous Idle            |
| 23  | 027 | 17  | 0010111     | ETB    | &#23;       |           | End of Transmission Block   |
| 24  | 030 | 18  | 0011000     | CAN    | &#24;       |           | Cancel                      |
| 25  | 031 | 19  | 0011001     | EM     | &#25;       |           | End of medium               |
| 26  | 032 | 1A  | 0011010     | SUB    | &#26;       |           | Substitute                  |
| 27  | 033 | 1B  | 0011011     | ESC    | &#27;       |           | Escape                      |
| 28  | 034 | 1C  | 0011100     | FS     | &#28;       |           | File Separator              |
| 29  | 035 | 1D  | 0011101     | GS     | &#29;       |           | Group Separator             |
| 30  | 036 | 1E  | 0011110     | RS     | &#30;       |           | Record Separator            |
| 31  | 037 | 1F  | ==0011111== | US     | &#31;       |           | Unit Separator              |

## ASCII udskrivbare tegn (kode 32-126)
[[#Indhold]]

ASCII-koderne **32–126** er de udskrivbare tegn.

De omfatter blandt andet:

- mellemrum
- cifrene `0–9`
- bogstaverne `A–Z`
- bogstaverne `a–z`
- tegnsætning
- matematiske og øvrige symboler

Eksempel:

```
A = decimal 65
A = hexadecimal 41
A = binær 1000001
```

Hvis værdien vises som en byte på otte bit, kan den skrives:

```
01000001
```

Kode **127** er ikke et udskrivbart tegn. Den repræsenterer kontroltegnet `DEL`.

| DEC | OCT | HEX | BIN     | Symbol  | HTML Number | HTML Name | Description                            |
| --- | --- | --- | ------- | ------- | ----------- | --------- | :------------------------------------- |
| 32  | 040 | 20  | 0100000 | SP      | &#32;       |           | Space                                  |
| 33  | 041 | 21  | 0100001 | !       | &#33;       | &excl;    | Exclamation mark                       |
| 34  | 042 | 22  | 0100010 | "       | &#34;       | &quot;    | Double quotes (or speech marks)        |
| 35  | 043 | 23  | 0100011 | #       | &#35;       | &num;     | Number sign                            |
| 36  | 044 | 24  | 0100100 | $       | &#36;       | &dollar;  | Dollar                                 |
| 37  | 045 | 25  | 0100101 | %       | &#37;       | &percnt;  | Per cent sign                          |
| 38  | 046 | 26  | 0100110 | &       | &#38;       | &amp;     | Ampersand                              |
| 39  | 047 | 27  | 0100111 | '       | &#39;       | &apos;    | Single quote                           |
| 40  | 050 | 28  | 0101000 | (       | &#40;       | &lparen;  | Open parenthesis (or open bracket)     |
| 41  | 051 | 29  | 0101001 | )       | &#41;       | &rparen;  | Close parenthesis (or close bracket)   |
| 42  | 052 | 2A  | 0101010 | *       | &#42;       | &ast;     | Asterisk                               |
| 43  | 053 | 2B  | 0101011 | +       | &#43;       | &plus;    | Plus                                   |
| 44  | 054 | 2C  | 0101100 | ,       | &#44;       | &comma;   | Comma                                  |
| 45  | 055 | 2D  | 0101101 | -       | &#45;       |           | Hyphen-minus                           |
| 46  | 056 | 2E  | 0101110 | .       | &#46;       | &period;  | Period, dot or full stop               |
| 47  | 057 | 2F  | 0101111 | /       | &#47;       | &sol;     | Slash or divide                        |
| 48  | 060 | 30  | 0110000 | 0       | &#48;       |           | Zero                                   |
| 49  | 061 | 31  | 0110001 | 1       | &#49;       |           | One                                    |
| 50  | 062 | 32  | 0110010 | 2       | &#50;       |           | Two                                    |
| 51  | 063 | 33  | 0110011 | 3       | &#51;       |           | Three                                  |
| 52  | 064 | 34  | 0110100 | 4       | &#52;       |           | Four                                   |
| 53  | 065 | 35  | 0110101 | 5       | &#53;       |           | Five                                   |
| 54  | 066 | 36  | 0110110 | 6       | &#54;       |           | Six                                    |
| 55  | 067 | 37  | 0110111 | 7       | &#55;       |           | Seven                                  |
| 56  | 070 | 38  | 0111000 | 8       | &#56;       |           | Eight                                  |
| 57  | 071 | 39  | 0111001 | 9       | &#57;       |           | Nine                                   |
| 58  | 072 | 3A  | 0111010 | :       | &#58;       | &colon;   | Colon                                  |
| 59  | 073 | 3B  | 0111011 | ;       | &#59;       | &semi;    | Semicolon                              |
| 60  | 074 | 3C  | 0111100 | <       | &#60;       | &lt;      | Less than (or open angled bracket)     |
| 61  | 075 | 3D  | 0111101 | =       | &#61;       | &equals;  | Equals                                 |
| 62  | 076 | 3E  | 0111110 | >       | &#62;       | &gt;      | Greater than (or close angled bracket) |
| 63  | 077 | 3F  | 0111111 | ?       | &#63;       | &quest;   | Question mark                          |
| 64  | 100 | 40  | 1000000 | @       | &#64;       | &commat;  | At sign                                |
| 65  | 101 | 41  | 1000001 | A       | &#65;       |           | Uppercase A                            |
| 66  | 102 | 42  | 1000010 | B       | &#66;       |           | Uppercase B                            |
| 67  | 103 | 43  | 1000011 | C       | &#67;       |           | Uppercase C                            |
| 68  | 104 | 44  | 1000100 | D       | &#68;       |           | Uppercase D                            |
| 69  | 105 | 45  | 1000101 | E       | &#69;       |           | Uppercase E                            |
| 70  | 106 | 46  | 1000110 | F       | &#70;       |           | Uppercase F                            |
| 71  | 107 | 47  | 1000111 | G       | &#71;       |           | Uppercase G                            |
| 72  | 110 | 48  | 1001000 | H       | &#72;       |           | Uppercase H                            |
| 73  | 111 | 49  | 1001001 | I       | &#73;       |           | Uppercase I                            |
| 74  | 112 | 4A  | 1001010 | J       | &#74;       |           | Uppercase J                            |
| 75  | 113 | 4B  | 1001011 | K       | &#75;       |           | Uppercase K                            |
| 76  | 114 | 4C  | 1001100 | L       | &#76;       |           | Uppercase L                            |
| 77  | 115 | 4D  | 1001101 | M       | &#77;       |           | Uppercase M                            |
| 78  | 116 | 4E  | 1001110 | N       | &#78;       |           | Uppercase N                            |
| 79  | 117 | 4F  | 1001111 | O       | &#79;       |           | Uppercase O                            |
| 80  | 120 | 50  | 1010000 | P       | &#80;       |           | Uppercase P                            |
| 81  | 121 | 51  | 1010001 | Q       | &#81;       |           | Uppercase Q                            |
| 82  | 122 | 52  | 1010010 | R       | &#82;       |           | Uppercase R                            |
| 83  | 123 | 53  | 1010011 | S       | &#83;       |           | Uppercase S                            |
| 84  | 124 | 54  | 1010100 | T       | &#84;       |           | Uppercase T                            |
| 85  | 125 | 55  | 1010101 | U       | &#85;       |           | Uppercase U                            |
| 86  | 126 | 56  | 1010110 | V       | &#86;       |           | Uppercase V                            |
| 87  | 127 | 57  | 1010111 | W       | &#87;       |           | Uppercase W                            |
| 88  | 130 | 58  | 1011000 | X       | &#88;       |           | Uppercase X                            |
| 89  | 131 | 59  | 1011001 | Y       | &#89;       |           | Uppercase Y                            |
| 90  | 132 | 5A  | 1011010 | Z       | &#90;       |           | Uppercase Z                            |
| 91  | 133 | 5B  | 1011011 | [       | &#91;       | &lsqb;    | Opening bracket                        |
| 92  | 134 | 5C  | 1011100 | \|&#92; | &bsol;      | Backslash |                                        |
| 93  | 135 | 5D  | 1011101 | ]       | &#93;       | &rsqb;    | Closing bracket                        |
| 94  | 136 | 5E  | 1011110 | ^       | &#94;       | &Hat;     | Caret - circumflex                     |
| 95  | 137 | 5F  | 1011111 | _       | &#95;       | &lowbar;  | Underscore                             |
| 96  | 140 | 60  | 1100000 | `       | &#96;       | &grave;   | Grave accent                           |
| 97  | 141 | 61  | 1100001 | a       | &#97;       |           | Lowercase a                            |
| 98  | 142 | 62  | 1100010 | b       | &#98;       |           | Lowercase b                            |
| 99  | 143 | 63  | 1100011 | c       | &#99;       |           | Lowercase c                            |
| 100 | 144 | 64  | 1100100 | d       | &#100;      |           | Lowercase d                            |
| 101 | 145 | 65  | 1100101 | e       | &#101;      |           | Lowercase e                            |
| 102 | 146 | 66  | 1100110 | f       | &#102;      |           | Lowercase f                            |
| 103 | 147 | 67  | 1100111 | g       | &#103;      |           | Lowercase g                            |
| 104 | 150 | 68  | 1101000 | h       | &#104;      |           | Lowercase h                            |
| 105 | 151 | 69  | 1101001 | i       | &#105;      |           | Lowercase i                            |
| 106 | 152 | 6A  | 1101010 | j       | &#106;      |           | Lowercase j                            |
| 107 | 153 | 6B  | 1101011 | k       | &#107;      |           | Lowercase k                            |
| 108 | 154 | 6C  | 1101100 | l       | &#108;      |           | Lowercase l                            |
| 109 | 155 | 6D  | 1101101 | m       | &#109;      |           | Lowercase m                            |
| 110 | 156 | 6E  | 1101110 | n       | &#110;      |           | Lowercase n                            |
| 111 | 157 | 6F  | 1101111 | o       | &#111;      |           | Lowercase o                            |
| 112 | 160 | 70  | 1110000 | p       | &#112;      |           | Lowercase p                            |
| 113 | 161 | 71  | 1110001 | q       | &#113;      |           | Lowercase q                            |
| 114 | 162 | 72  | 1110010 | r       | &#114;      |           | Lowercase r                            |
| 115 | 163 | 73  | 1110011 | s       | &#115;      |           | Lowercase s                            |
| 116 | 164 | 74  | 1110100 | t       | &#116;      |           | Lowercase t                            |
| 117 | 165 | 75  | 1110101 | u       | &#117;      |           | Lowercase u                            |
| 118 | 166 | 76  | 1110110 | v       | &#118;      |           | Lowercase v                            |
| 119 | 167 | 77  | 1110111 | w       | &#119;      |           | Lowercase w                            |
| 120 | 170 | 78  | 1111000 | x       | &#120;      |           | Lowercase x                            |
| 121 | 171 | 79  | 1111001 | y       | &#121;      |           | Lowercase y                            |
| 122 | 172 | 7A  | 1111010 | z       | &#122;      |           | Lowercase z                            |
| 123 | 173 | 7B  | 1111011 | {       | &#123;      | &lcub;    | Opening brace                          |
| 124 | 174 | 7C  | 1111100 | \|      | &#124;      | &verbar;  | Vertical bar                           |
| 125 | 175 | 7D  | 1111101 | }       | &#125;      | &rcub;    | Closing brace                          |
| 126 | 176 | 7E  | 1111110 | ~       | &#126;      | &tilde;   | Equivalency sign - tilde               |
| 127 | 177 | 7F  | 1111111 | DEL     | &#127;      |           | Delete                                 |

ASCII havde kun 128 mulige værdier. Efterhånden som computere blev udbredt internationalt, opstod der behov for langt flere tegn end dem, der fandtes i den oprindelige ASCII-standard.

Den tekniske udvikling medførte at mange computersystemer begyndte at arbejded med 8-bit-bytes.

Med 8 bit findes: $2^8 = 256$ mulige værdier.

Det gjorde det muligt at anvende værdierne 128–255 til yderligere tegn. Problemet var imidlertid, at forskellige producenter og lande definerede disse værdier forskelligt.

Dermed opstod forskellige **codepages**.

## 8-bit-codepages og såkaldt "udvidet ASCII"
[[#Indhold]]

Med de 8 bit blev det muligt at lave flere codepages, som blev tilpasset de forskellige formål.

Begrebet **udvidet ASCII** (_extended ASCII_) anvendes ofte om 8-bit-tegnkodninger, hvor ASCII's værdier 0–127 bevares, mens værdierne 128–255 anvendes til yderligere tegn.

Det er vigtigt at være opmærksom på, at **extended ASCII ikke er én bestemt standard**.

Der findes mange forskellige 8-bit-codepages, eksempelvis:

- Windows-1252
- ISO-8859-1
- IBM Code Page 437
- Windows-1250

Det betyder, at byteværdien eksempelvis `0x80` ikke nødvendigvis repræsenterer det samme tegn i forskellige codepages.

### Windows-1252

Tabellen herunder viser **Windows-1252 (CP1252)**.

Windows-1252 blev især anvendt til vesteuropæiske sprog i Microsoft Windows.

Windows-1252 og ISO-8859-1 ligner hinanden, men de er **ikke identiske**. Området `0x80–0x9F` er en væsentlig forske mellem de to tegnkodninger.

Nedenstående tabel er Windows-1252 (CP-1252), som er et såkaldt superset af ISO 8859-1-standarden, også kaldet ISO Latin-1.

| DEC | OCT | HEX | BIN      | Symbol | HTML Number | HTML Name | Description                                |
| --- | --- | --- | -------- | ------ | ----------- | --------- | :----------------------------------------- |
| 128 | 200 | 80  | 10000000 | €      | &#8364;     | &euro;    | Euro sign                                  |
| 129 | 201 | 81  | 10000001 |        |             |           | Unused                                     |
| 130 | 202 | 82  | 10000010 | ‚      | &#130;      | &sbquo;   | Single low-9 quotation mark                |
| 131 | 203 | 83  | 10000011 | ƒ      | &#131;      | &fnof;    | Latin small letter f with hook             |
| 132 | 204 | 84  | 10000100 | „      | &#132;      | &bdquo;   | Double low-9 quotation mark                |
| 133 | 205 | 85  | 10000101 | …      | &#133;      | &hellip;  | Horizontal ellipsis                        |
| 134 | 206 | 86  | 10000110 | †      | &#134;      | &dagger;  | Dagger                                     |
| 135 | 207 | 87  | 10000111 | ‡      | &#135;      | &Dagger;  | Double dagger                              |
| 136 | 210 | 88  | 10001000 | ˆ      | &#136;      | &circ;    | Modifier letter circumflex accent          |
| 137 | 211 | 89  | 10001001 | ‰      | &#137;      | &permil;  | Per mille sign                             |
| 138 | 212 | 8A  | 10001010 | Š      | &#138;      | &Scaron;  | Latin capital letter S with caron          |
| 139 | 213 | 8B  | 10001011 | ‹      | &#139;      | &lsaquo;  | Single left-pointing angle quotation       |
| 140 | 214 | 8C  | 10001100 | Œ      | &#140;      | &OElig;   | Latin capital ligature OE                  |
| 141 | 215 | 8D  | 10001101 |        |             |           | Unused                                     |
| 142 | 216 | 8E  | 10001110 | Ž      | &#142;      | &Zcaron;  | Latin capital letter Z with caron          |
| 143 | 217 | 8F  | 10001111 |        |             |           | Unused                                     |
| 144 | 220 | 90  | 10010000 |        |             |           | Unused                                     |
| 145 | 221 | 91  | 10010001 | ‘      | &#145;      | &lsquo;   | Left single quotation mark                 |
| 146 | 222 | 92  | 10010010 | ’      | &#146;      | &rsquo;   | Right single quotation mark                |
| 147 | 223 | 93  | 10010011 | “      | &#147;      | &ldquo;   | Left double quotation mark                 |
| 148 | 224 | 94  | 10010100 | ”      | &#148;      | &rdquo;   | Right double quotation mark                |
| 149 | 225 | 95  | 10010101 | •      | &#149;      | &bull;    | Bullet                                     |
| 150 | 226 | 96  | 10010110 | –      | &#150;      | &ndash;   | En dash                                    |
| 151 | 227 | 97  | 10010111 | —      | &#151;      | &mdash;   | Em dash                                    |
| 152 | 230 | 98  | 10011000 | ˜      | &#152;      | &tilde;   | Small tilde                                |
| 153 | 231 | 99  | 10011001 | ™      | &#153;      | &trade;   | Trade mark sign                            |
| 154 | 232 | 9A  | 10011010 | š      | &#154;      | &scaron;  | Latin small letter S with caron            |
| 155 | 233 | 9B  | 10011011 | ›      | &#155;      | &rsaquo;  | Single right-pointing angle quotation mark |
| 156 | 234 | 9C  | 10011100 | œ      | &#156;      | &oelig;   | Latin small ligature oe                    |
| 157 | 235 | 9D  | 10011101 |        |             |           | Unused                                     |
| 158 | 236 | 9E  | 10011110 | ž      | &#158;      | &zcaron;  | Latin small letter z with caron            |
| 159 | 237 | 9F  | 10011111 | Ÿ      | &#159;      | &Yuml;    | Latin capital letter Y with diaeresis      |
| 160 | 240 | A0  | 10100000 | NBSP   | &#160;      | &nbsp;    | Non-breaking space                         |
| 161 | 241 | A1  | 10100001 | ¡      | &#161;      | &iexcl;   | Inverted exclamation mark                  |
| 162 | 242 | A2  | 10100010 | ¢      | &#162;      | &cent;    | Cent sign                                  |
| 163 | 243 | A3  | 10100011 | £      | &#163;      | &pound;   | Pound sign                                 |
| 164 | 244 | A4  | 10100100 | ¤      | &#164;      | &curren;  | Currency sign                              |
| 165 | 245 | A5  | 10100101 | ¥      | &#165;      | &yen;     | Yen sign                                   |
| 166 | 246 | A6  | 10100110 | ¦      | &#166;      | &brvbar;  | Pipe, broken vertical bar                  |
| 167 | 247 | A7  | 10100111 | §      | &#167;      | &sect;    | Section sign                               |
| 168 | 250 | A8  | 10101000 | ¨      | &#168;      | &uml;     | Spacing diaeresis - umlaut                 |
| 169 | 251 | A9  | 10101001 | ©      | &#169;      | &copy;    | Copyright sign                             |
| 170 | 252 | AA  | 10101010 | ª      | &#170;      | &ordf;    | Feminine ordinal indicator                 |
| 171 | 253 | AB  | 10101011 | «      | &#171;      | &laquo;   | Left double angle quotes                   |
| 172 | 254 | AC  | 10101100 | ¬      | &#172;      | &not;     | Negation                                   |
| 173 | 255 | AD  | 10101101 | ­SHY   | &#173;      | &shy;     | Soft hyphen                                |
| 174 | 256 | AE  | 10101110 | ®      | &#174;      | &reg;     | Registered trade mark sign                 |
| 175 | 257 | AF  | 10101111 | ¯      | &#175;      | &macr;    | Spacing macron - overline                  |
| 176 | 260 | B0  | 10110000 | °      | &#176;      | &deg;     | Degree sign                                |
| 177 | 261 | B1  | 10110001 | ±      | &#177;      | &plusmn;  | Plus-or-minus sign                         |
| 178 | 262 | B2  | 10110010 | ²      | &#178;      | &sup2;    | Superscript two - squared                  |
| 179 | 263 | B3  | 10110011 | ³      | &#179;      | &sup3;    | Superscript three - cubed                  |
| 180 | 264 | B4  | 10110100 | ´      | &#180;      | &acute;   | Acute accent - spacing acute               |
| 181 | 265 | B5  | 10110101 | µ      | &#181;      | &micro;   | Micro sign                                 |
| 182 | 266 | B6  | 10110110 | ¶      | &#182;      | &para;    | Pilcrow sign - paragraph sign              |
| 183 | 267 | B7  | 10110111 | ·      | &#183;      | &middot;  | Middle dot - Georgian comma                |
| 184 | 270 | B8  | 10111000 | ¸      | &#184;      | &cedil;   | Spacing cedilla                            |
| 185 | 271 | B9  | 10111001 | ¹      | &#185;      | &sup1;    | Superscript one                            |
| 186 | 272 | BA  | 10111010 | º      | &#186;      | &ordm;    | Masculine ordinal indicator                |
| 187 | 273 | BB  | 10111011 | »      | &#187;      | &raquo;   | Right double angle quotes                  |
| 188 | 274 | BC  | 10111100 | ¼      | &#188;      | &frac14;  | Fraction one quarter                       |
| 189 | 275 | BD  | 10111101 | ½      | &#189;      | &frac12;  | Fraction one half                          |
| 190 | 276 | BE  | 10111110 | ¾      | &#190;      | &frac34;  | Fraction three quarters                    |
| 191 | 277 | BF  | 10111111 | ¿      | &#191;      | &iquest;  | Inverted question mark                     |
| 192 | 300 | C0  | 11000000 | À      | &#192;      | &Agrave;  | Latin capital letter A with grave          |
| 193 | 301 | C1  | 11000001 | Á      | &#193;      | &Aacute;  | Latin capital letter A with acute          |
| 194 | 302 | C2  | 11000010 | Â      | &#194;      | &Acirc;   | Latin capital letter A with circumflex     |
| 195 | 303 | C3  | 11000011 | Ã      | &#195;      | &Atilde;  | Latin capital letter A with tilde          |
| 196 | 304 | C4  | 11000100 | Ä      | &#196;      | &Auml;    | Latin capital letter A with diaeresis      |
| 197 | 305 | C5  | 11000101 | Å      | &#197;      | &Aring;   | Latin capital letter A with ring above     |
| 198 | 306 | C6  | 11000110 | Æ      | &#198;      | &AElig;   | Latin capital letter AE                    |
| 199 | 307 | C7  | 11000111 | Ç      | &#199;      | &Ccedil;  | Latin capital letter C with cedilla        |
| 200 | 310 | C8  | 11001000 | È      | &#200;      | &Egrave;  | Latin capital letter E with grave          |
| 201 | 311 | C9  | 11001001 | É      | &#201;      | &Eacute;  | Latin capital letter E with acute          |
| 202 | 312 | CA  | 11001010 | Ê      | &#202;      | &Ecirc;   | Latin capital letter E with circumflex     |
| 203 | 313 | CB  | 11001011 | Ë      | &#203;      | &Euml;    | Latin capital letter E with diaeresis      |
| 204 | 314 | CC  | 11001100 | Ì      | &#204;      | &Igrave;  | Latin capital letter I with grave          |
| 205 | 315 | CD  | 11001101 | Í      | &#205;      | &Iacute;  | Latin capital letter I with acute          |
| 206 | 316 | CE  | 11001110 | Î      | &#206;      | &Icirc;   | Latin capital letter I with circumflex     |
| 207 | 317 | CF  | 11001111 | Ï      | &#207;      | &Iuml;    | Latin capital letter I with diaeresis      |
| 208 | 320 | D0  | 11010000 | Ð      | &#208;      | &ETH;     | Latin capital letter ETH                   |
| 209 | 321 | D1  | 11010001 | Ñ      | &#209;      | &Ntilde;  | Latin capital letter N with tilde          |
| 210 | 322 | D2  | 11010010 | Ò      | &#210;      | &Ograve;  | Latin capital letter O with grave          |
| 211 | 323 | D3  | 11010011 | Ó      | &#211;      | &Oacute;  | Latin capital letter O with acute          |
| 212 | 324 | D4  | 11010100 | Ô      | &#212;      | &Ocirc;   | Latin capital letter O with circumflex     |
| 213 | 325 | D5  | 11010101 | Õ      | &#213;      | &Otilde;  | Latin capital letter O with tilde          |
| 214 | 326 | D6  | 11010110 | Ö      | &#214;      | &Ouml;    | Latin capital letter O with diaeresis      |
| 215 | 327 | D7  | 11010111 | ×      | &#215;      | &times;   | Multiplication sign                        |
| 216 | 330 | D8  | 11011000 | Ø      | &#216;      | &Oslash;  | Latin capital letter O with slash          |
| 218 | 332 | DA  | 11011010 | Ú      | &#218;      | &Uacute;  | Latin capital letter U with acute          |
| 217 | 331 | D9  | 11011001 | Ù      | &#217;      | &Ugrave;  | Latin capital letter U with grave          |
| 219 | 333 | DB  | 11011011 | Û      | &#219;      | &Ucirc;   | Latin capital letter U with circumflex     |
| 220 | 334 | DC  | 11011100 | Ü      | &#220;      | &Uuml;    | Latin capital letter U with diaeresis      |
| 221 | 335 | DD  | 11011101 | Ý      | &#221;      | &Yacute;  | Latin capital letter Y with acute          |
| 222 | 336 | DE  | 11011110 | Þ      | &#222;      | &THORN;   | Latin capital letter THORN                 |
| 223 | 337 | DF  | 11011111 | ß      | &#223;      | &szlig;   | Latin small letter sharp s - ess-zed       |
| 224 | 340 | E0  | 11100000 | à      | &#224;      | &agrave;  | Latin small letter a with grave            |
| 225 | 341 | E1  | 11100001 | á      | &#225;      | &aacute;  | Latin small letter a with acute            |
| 226 | 342 | E2  | 11100010 | â      | &#226;      | &acirc;   | Latin small letter a with circumflex       |
| 227 | 343 | E3  | 11100011 | ã      | &#227;      | &atilde;  | Latin small letter a with tilde            |
| 228 | 344 | E4  | 11100100 | ä      | &#228;      | &auml;    | Latin small letter a with diaeresis        |
| 229 | 345 | E5  | 11100101 | å      | &#229;      | &aring;   | Latin small letter a with ring above       |
| 230 | 346 | E6  | 11100110 | æ      | &#230;      | &aelig;   | Latin small letter ae                      |
| 231 | 347 | E7  | 11100111 | ç      | &#231;      | &ccedil;  | Latin small letter c with cedilla          |
| 232 | 350 | E8  | 11101000 | è      | &#232;      | &egrave;  | Latin small letter e with grave            |
| 233 | 351 | E9  | 11101001 | é      | &#233;      | &eacute;  | Latin small letter e with acute            |
| 234 | 352 | EA  | 11101010 | ê      | &#234;      | &ecirc;   | Latin small letter e with circumflex       |
| 235 | 353 | EB  | 11101011 | ë      | &#235;      | &euml;    | Latin small letter e with diaeresis        |
| 236 | 354 | EC  | 11101100 | ì      | &#236;      | &igrave;  | Latin small letter i with grave            |
| 237 | 355 | ED  | 11101101 | í      | &#237;      | &iacute;  | Latin small letter i with acute            |
| 238 | 356 | EE  | 11101110 | î      | &#238;      | &icirc;   | Latin small letter i with circumflex       |
| 239 | 357 | EF  | 11101111 | ï      | &#239;      | &iuml;    | Latin small letter i with diaeresis        |
| 240 | 360 | F0  | 11110000 | ð      | &#240;      | &eth;     | Latin small letter eth                     |
| 241 | 361 | F1  | 11110001 | ñ      | &#241;      | &ntilde;  | Latin small letter n with tilde            |
| 242 | 362 | F2  | 11110010 | ò      | &#242;      | &ograve;  | Latin small letter o with grave            |
| 243 | 363 | F3  | 11110011 | ó      | &#243;      | &oacute;  | Latin small letter o with acute            |
| 244 | 364 | F4  | 11110100 | ô      | &#244;      | &ocirc;   | Latin small letter o with circumflex       |
| 245 | 365 | F5  | 11110101 | õ      | &#245;      | &otilde;  | Latin small letter o with tilde            |
| 246 | 366 | F6  | 11110110 | ö      | &#246;      | &ouml;    | Latin small letter o with diaeresis        |
| 247 | 367 | F7  | 11110111 | ÷      | &#247;      | &divide;  | Division sign                              |
| 248 | 370 | F8  | 11111000 | ø      | &#248;      | &oslash;  | Latin small letter o with slash            |
| 249 | 371 | F9  | 11111001 | ù      | &#249;      | &ugrave;  | Latin small letter u with grave            |
| 250 | 372 | FA  | 11111010 | ú      | &#250;      | &uacute;  | Latin small letter u with acute            |
| 251 | 373 | FB  | 11111011 | û      | &#251;      | &ucirc;   | Latin small letter u with circumflex       |
| 252 | 374 | FC  | 11111100 | ü      | &#252;      | &uuml;    | Latin small letter u with diaeresis        |
| 253 | 375 | FD  | 11111101 | ý      | &#253;      | &yacute;  | Latin small letter y with acute            |
| 254 | 376 | FE  | 11111110 | þ      | &#254;      | &thorn;   | Latin small letter thorn                   |
| 255 | 377 | FF  | 11111111 | ÿ      | &#255;      | &yuml;    | Latin small letter y with diaeresis        |

Problemet med codepages er grundlæggende, at et program skal vide, **hvilken tegnkodning en byteværdi skal fortolkes med**.

Eksempelvis kan:

```
11101000
```

ikke i sig selv fortælle programmet, hvilket tegn der menes.

Programmet skal også kende den anvendte tegnkodning.

Dette er en af årsagerne til, at moderne systemer i vid udstrækning anvender **Unicode**, typisk kodet som eksempelvis UTF-8.
# Præsentation
[[#Indhold]]

At repræsentere tegn er én problemstilling. At bestemme, **hvordan teksten skal præsenteres**, er en anden.

En tegnkodning som ASCII eller UTF-8 fortæller eksempelvis, hvilke tegn en række bytes repræsenterer. Den fortæller derimod ikke nødvendigvis:

- hvor stor teksten skal være
- om teksten skal være fed
- hvilken skrifttype der skal anvendes
- hvor et billede skal placeres
- hvordan en overskrift skal præsenteres

Til dette anvendes forskellige dokument- og markupformater.

Programmer som Microsoft Word kan tilbyde meget avancerede muligheder for opsætning og præsentation. Til gengæld bliver dokumentformatet mere komplekst end en almindelig tekstfil.

Der findes derfor forskellige formater med forskellige kompromiser mellem:

- enkelhed
- læsbarhed
- præsentationsmuligheder
- portabilitet
- maskinlæsbarhed
- mulighed for redigering i forskellige programmer

Et eksempel kan illustreres således:

| Filbeskrivelse             | Filtype | Eksempel       | Vurdering af præsentationsmuligheder<br><br>(Sammenholdt med hvorvidt det kan deles med andre programmer og platforme) |
| -------------------------- | ------- | -------------- | ---------------------------------------------------------------------------------------------------------------------- |
| Ren tekster                | txt     | filnavn.txt    | Meget lav                                                                                                              |
| ==Mark Down==              | md      | filnavn.md     | medium - men tilstrækkelig                                                                                             |
| Hypertext Markup Language  | HTML    | filnavn.html   | høj, men besværlig                                                                                                     |
| Extensible Markup Language | XML     | filnavn.xml    | høj, men meget besværlig                                                                                               |
| ...                        |         |                |                                                                                                                        |
| Microsoft Word filer       | docx    | filnavn.docx   | Høj, men meget låst til Office pakker                                                                                  |
| Draw.io filer              | drawio  | filnavn.drawio | Høj, men særdeles låst til Draw.io                                                                                     |

Et draw.io-diagram kan eksempelvis eksporteres som PNG eller SVG og indsættes i Word. Men Word forstår ikke nødvendigvis den interne draw.io-model på samme måde, som draw.io selv gør.

Man mister derfor typisk noget redigerbarhed eller integration, når indhold flyttes mellem forskellige specialiserede programmer.

Markdown forsøger at placere sig et andet sted i dette kompromis.

Markdown giver ikke de samme layoutmuligheder som eksempelvis Word eller HTML med CSS. Til gengæld er en Markdown-fil grundlæggende en almindelig tekstfil, som kan læses og redigeres i mange forskellige programmer og på mange forskellige operativsystemer.


<div style="page-break-after: always; visibility: hidden">\pagebreak\</div>
# Kildehenvisninger
[[#Indhold]]

https://en.wikipedia.org/wiki/Telegraph_code

https://en.wikipedia.org/wiki/American_Morse_code

https://en.wikipedia.org/wiki/Morse_code

https://da.wikipedia.org/wiki/Telegrafi

https://www.cryptomuseum.com/ref/ita2/index.htm

https://www.ascii-code.com/

https://www.markdownguide.org/extended-syntax/


https://www.youtube.com/shorts/9DCP4TMYg_M

https://youtu.be/KrzJqC_RtSU

https://www.youtube.com/shorts/C2GdPW10leE
<a href="https://mr.varmen.rs/"><img src="media/cover.jpg" alt="Mr. Varmen, naslovna strana na laptopu i telefonu" width="100%"></a>

# Mr. Varmen

Sajt mobilnog koktel bara za svadbe, rođendane i poslovne događaje, sa filmom na početnoj koji se odvija dok se skroluje.

**[mr.varmen.rs](https://mr.varmen.rs/)** · [Studija slučaja](https://svilenkovic.rs/radovi/mr-varmen) · [English](README.md)

> [!NOTE]
> Klijentski projekat. Izvorni kod pripada klijentu i čuva se u privatnom repozitorijumu. Ova stranica opisuje šta sam uradio i kako.

<table>
  <tr><td><b>Klijent</b></td><td>Mr. Varmen</td></tr>
  <tr><td><b>Delatnost</b></td><td>Mobilni koktel bar za događaje</td></tr>
  <tr><td><b>Lokacija</b></td><td>Leskovac, Niš i Beograd</td></tr>
  <tr><td><b>Vrsta</b></td><td>Sajt sa više strana</td></tr>
  <tr><td><b>Moj deo posla</b></td><td>Dizajn, izrada, SEO, hosting i održavanje</td></tr>
  <tr><td><b>Tehnologije</b></td><td>Astro, JavaScript, PHP, JSON-LD</td></tr>
</table>

## O projektu

Mr. Varmen dovodi ceo koktel bar sa barmenom na svadbe, rođendane i poslovne događaje u Leskovcu, Nišu, Beogradu i okolnim gradovima. Mobilni bar se ne bira sa spiska koktela, pa sajt prvo pokazuje pripremu i sipanje, a tek onda ponudu. Odatle vodi do kratkog razgovora o datumu, broju gostiju i meniju.

Početna se otvara filmom zakačenim za ekran, u četiri poglavlja. Na desktopu položaj skrola određuje trenutak snimka, na ekranima na dodir se u petlji vrti posebna verzija za telefon, a natpisi i traka poglavlja u oba slučaja prate skrol. Ništa se ne preuzima do prvog skrola ili dodira, ili dok ne prođe šest sekundi. Uz uključenu uštedu podataka video se nikad ne učitava, a ko je tražio smanjen pokret dobija poster i tekst.

## Šta sam uradio

- Posebne strane za svadbe, rođendane, poslovne događaje i Niš sa okolinom, plus blog sa pet praktičnih tekstova
- Rezervacija u tri koraka (razgovor, predlog menija, samo veče) i forma za datum, broj gostiju, vrstu događaja i mesto
- Mala PHP skripta iza forme, sa zaštitom od botova i jasnom potvrdom posetiocu
- Raspored filma postavlja mala skripta u samoj strani pre prvog iscrtavanja, pa uvod ne skače dok se strana učitava
- Petlja animacije radi samo dok je film na ekranu, a to prati IntersectionObserver
- Statične strane iz Astra, a pravne strane i podešavanja kolačića izgledaju kao ostatak sajta

## Merenja

| | Performanse | Pristupačnost | Dobre prakse | SEO |
| :-- | :-: | :-: | :-: | :-: |
| Telefon | 98 | 100 | 100 | 100 |
| Desktop | 97 | 100 | 100 | 100 |

PageSpeed Insights, laboratorijsko merenje živog sajta, septembar 2026. Sigurnosna zaglavlja: 6 od 6. HTML validator: bez grešaka. axe provera pristupačnosti: bez prekršaja. Strukturisani podaci: `FAQPage`, `LocalBusiness`, `Service`.

## Snimci ekrana

<table>
  <tr>
    <td width="68%" valign="top"><img src="media/desktop.webp" alt="Mr. Varmen, naslovna strana na ekranu širine 1440 px"></td>
    <td width="32%" valign="top"><img src="media/mobile.webp" alt="Mr. Varmen, naslovna strana na telefonu"></td>
  </tr>
</table>

<img src="media/inner-1.webp" alt="Ponuda je podeljena prema vrsti događaja i formatu bara">
<sub>Ponuda je podeljena prema vrsti događaja i formatu bara</sub>

<img src="media/inner-2.webp" alt="Blog sa praktičnim savetima za izbor i organizaciju bara">
<sub>Blog sa praktičnim savetima za izbor i organizaciju bara</sub>

---

<sub>Izrada: [D. Svilenković](https://svilenkovic.rs).</sub>

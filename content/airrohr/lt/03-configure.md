---
title: Konfigūruoti
---

### Gaukite unikalų stoties ID
1. Prijunkite stotį prie USB kabelio, kad jutiklis būtų įjungtas.

2. Stotis bandys prisijungti prie sukonfigūruoto "WiFi" tinklo. Naujai sukonfigūravus, prisijungti nepavyks ir stotis sukurs "WiFi" tinklą su pavadinimu `Particulate Matter ID` , `Feinstaubsensor-ID` arba `airRohr-ID`. ID yra **ChipID** (pavyzdžiui, 13597771). **Prašome užsirašyti šį numerį, nes jis bus reikalingas registracijai**.

3. Kompiuteryje arba išmaniajame telefone prisijunkite prie stoties sukurto "WiFi" tinklo. Numatytasis šio tinklo slaptažodis yra `airrohrcfg`. Palaukite, kol bus užmegztas ryšys.<br>*Android*: Jei ryšys iš karto nutrūksta, gali tekti išjungti parinktį "Smart network switch" (išmanusis tinklo perjungimas), esančią skiltyje "Connections -> WiFi -> Advanced" (Ryšiai -> "WiFi" -> "Advanced").

4. Atidarykite naršyklę ir įveskite [http://192.168.4.1/](http://192.168.4.1/).

> ⚠️ **Atkreipkite dėmesį** Gali prireikti kelių bandymų, kad "NodeMCU" prisijungtų prie namų "WiFi" tinklo. Būkite kantrūs ir bandykite atlikti veiksmus kelis kartus, kol pavyks prisijungti. Jei jutiklio konfigūracija pavyko, stoties "WiFi" tinklas bus nepasiekiamas ir konfigūracijos puslapis nebebus pasiekiamas pagal šį IP 192.168.4.1

### Konfigūruokite stotį
1. Puslapyje "Configuration" (Konfigūracija) įveskite SSID (namų WiFi tinklo pavadinimą), tinklo saugumo raktą (sistemoje "Windows") arba WiFi slaptažodį.

2. Jei naudojate rekomenduojamą smulkių dulkių jutiklį (SDS011), jokių papildomų konfigūracijos pakeitimų atlikti nereikia.

3. Spustelėkite mygtuką "Save configuration and restart" (Išsaugoti konfigūraciją ir paleisti iš naujo). Stotis bus paleista iš naujo ir nebebus pasiekiama tokiu būdu, kai ji prisijungs prie jūsų namų WiFi tinklo.

<br>

<img src="../docs/airrohr_config_initial.jpg" loading="lazy"/>

<br>

### Patikrinkite, ar teisingai sukonfigūruota stotis
Jei ankstesniame žingsnyje neatlikote jokių kitų pakeitimų, išskyrus "WiFi" tinklo konfigūraciją, dabar jutiklis pradės įrašinėti ir siųsti duomenis. Maždaug po 10 minučių galite patikrinti, ar viskas veikia teisingai, pereidami į šiuos puslapius. Šiuose puslapiuose ieškokite ChipID (pirmiau pateiktame pavyzdyje - 13597771).

* [Jutiklio duomenys](https://www.madavi.de/sensor/graph.php)
* [WiFi signalo duomenys](https://www.madavi.de/sensor/signal.php)

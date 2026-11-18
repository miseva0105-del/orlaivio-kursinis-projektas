AMFIBIJOS MISIJOS IR SPECIFIKACIJŲ DEMONSTRATORIUS
Atnaujinta 2026-11-18

KAIP PRADĖTI
1. Išskleiskite visą ZIP. Failai index.html ir app.js turi likti tame pačiame aplanke.
2. Naršyklėje atverkite index.html. Etapus rinkitės viršuje arba mygtukais apačioje.
3. Atverkite Google Colab: https://colab.research.google.com/
4. File → Upload notebook (arba Open notebook → Upload): įkelkite
   Amfibijos_misija_su_ivadu.ipynb. Išsaugokite savo kopiją Google Drive.
5. Vykdykite kodo blokus nuo viršaus su ▶ arba Shift + Enter.

DARBO LOGIKA
Studentas apibrėžia užduotį ir duomenis → parašo užklausą ChatGPT,
kad sukurtų Python kodą → įklijuoja kodą į Colab → paleidžia → tikrina rezultatą.
Kiekviename taikymo etape pateikta konkreti užklausa, patikrintas pavyzdinis
kodas, jo išvestis ir studento veiksmas. Puslapis pats Python kodo nevykdo.
Užrašinėje jau yra pavyzdinės išvestys; pakeitus duomenis reikia paleisti kodą.

ANALOGŲ DUOMENŲ BAZĖ
Nuolatinis mygtukas viršuje atveria redaguojamą duomenų bazę:
- projekto atrankos kriterijai ir ribos;
- orlaivių palyginimas, tinkamumo vertinimas ir priežastys;
- atskiri parametrų įrašai su vienetais, sąlygomis ir šaltiniais.
Įrašai saugomi šioje naršyklėje, jei tai leidžiama.
Visada išsaugokite JSON kopiją; ją galima importuoti tame pačiame puslapyje.
CSV eksportas skirtas lentelėms. Duomenys į Colab savaime nepersikelia.
Užrašinės 4 etape yra pasirinktinis JSON importo blokas; norint jį naudoti,
IMPORTUOTI_BAZE pakeičiama į True ir pasirenkamas eksportuotas JSON.

PAVEIKSLAI IR SKAIČIAI
- Paprastas 2D profilis išlaikytas: tik trys skrydžio atkarpos, 120 km.
- Atskirame etape modelis papildytas riedėjimu, įsibėgėjimu ir lėtėjimu vandenyje.
- Erdvinė schema rodo visus šešis etapus; horizontalieji atstumai be mastelio.
- Greičio kitimo grafikai pašalinti. Supaprastintoms degalų sąnaudoms naudojamos
  atkarpų trukmės ir valandinės sąnaudos.
- Studentų platformoje nėra dėstytojo užsiėmimo plano.
- misija6 – šešių misijos etapų rezultatų lentelės kintamasis Python kode;
  instrukcijose vartojamas aiškus lentelės pavadinimas.
- Sąnaudos ir jautrumo analizė išlaikyti kaip papildomi žingsniai.
- Misijos skaičiai yra mokomosios prielaidos, o ne ICON A5 charakteristikos.
- 600 m tako ilgis nėra įsibėgėjimo kelias. Kinematinis palyginimas su taku
  nepatvirtina pilnos kilimo charakteristikos ar saugos.

KONTROLINIAI REZULTATAI
Skrydžio trys atkarpos: 120,000 km; 57,580886 min.
Papildyti šeši etapai: 121,003189 km; 59,259898 min.
Įsibėgėjimas nuo 18 iki 100 km/h, a=1,5 m/s²: 248,868 m; 15,185 s.
Lėtėjimas vandenyje nuo 110 iki 18 km/h, |a|=1 m/s²: 454,321 m; 25,556 s.
Greitėjimo, greičių ir 60 m pradinio aukštėjimo ribos prielaidos nėra patvirtinti
analogo duomenys; 60 m riba nenustato važiuoklės įtraukimo komandos.

REZULTATŲ IŠSAUGOJIMAS
Paskutiniuose blokuose kuriamas rezultatų ZIP. Užrašinę .ipynb išsaugokite atskirai.
HTML duomenų bazės JSON taip pat išsaugokite atskirai.
Aplanke rezultatai yra iš anksto apskaičiuoti CSV, PNG, SVG ir teksto pavyzdžiai.

KITOS JUPYTER APLINKOS
Tinka tas pats .ipynb failas. Jei aplinka meta konkrečią NumPy 1.x / 2.x
nesuderinamumo klaidą, atskirame bloke vykdykite:
%pip install "numpy<2"
Tada Kernel → Restart ir vėl vykdykite nuo pradžios.
Colab aplinkoje šio diegimo iš anksto atlikti nereikia.

METODIKOS PATIKSLINIMAS
Formulės HTML puslapyje pateiktos matematiškai (trupmenos, šaknys, indeksai),
o užrašinėje – LaTeX formatu. Prie jų paaiškinti dydžiai, vienetai, taikymo
sąlygos ir skaitiniai pavyzdžiai. Patikslintas grafikų užrašų fonas bei išdėstymas.

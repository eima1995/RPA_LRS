# Paleidimas:
Robotas priskiria failų atsisiuntimams darbinę direktoriją.
Naudojama IDE UIPATH.

# Veikimas:
Robotas atidaro nuorodą:
http://www.lrs.lt/pls/proj/dokpaieska.derinimui_l?p_org=18
1. Robotas atrenka einamosios dienos įrašus pagal data, numerį, tipą.
2. Robotas Pildo MS Excel Lentelę, kur nurodyti šie stulpeliai: Data, Numeris, Tipas, Gauta derinimui, Išvadas teikti iki, Statusas
3. Robotas atidaro Teisės akto nuorodą:
a. Išsaugo “Teisės akto projekto tekstas” spaudžiant Word ikoną.
b. Išsaugo susijusius dokumentus:
  - Pridėti dokumentai (išsaugomi visi pridėti dokumentai)
  - Susiję dokumentai (išsaugomi visi susiję dokumentai)
4. Visi dokumentai saugomi į katalogą. Katalogo struktūra: data (YYYY-MM-DD) > Dokumento Registracijos Numeris (pvz. 17-8757)
5. Visus sudėtus dokumentus robotas išsiunčia el. Paštu. El. Pastas turi būti imamas iš Tam skirto Excel, Parameters.xlsx. El. Laiško tema: Gautas naujas TA Reg. Nr. (nurodomas numeris). Laiško tekstas: “Laba diena, teikiame gautus derinti TA.”
6. Išsiuntus el. Laiškus su Teisės aktais robotas MS Excel lentelėjė ties kiekvienu įrašu pakeičia status į “Išsiųsta” 

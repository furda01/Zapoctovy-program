V přiloženém souboru se nachází devět funkcí, z nichž jedna je testem prvočíselnosti, tři vypočítávají největší společný dělitel, dva nejmensí společný násobek a poslední tři mají za úkol zjistit prvočíselný rozklad.

Pro funkci je_prvocislo zjišťující prvočíselnost daného čísla je potřebným vstupem intová proměnná větší nebo rovna 2 a výstupem je bool. Algoritmus použitý v této funkci je podobný Miller-Rabinovu testu prvočíselnosti, jak byl popsán v knize Umění programování 2.díl od Donalda Knutha. Přestože je to pravděpodobnostní test, tak v důsledku 25 opakování je pravděpodobnost nesprávného výsledku (asi 1:10^15) nižší než pravděpodobnost, že se uvnitř počítače změní hodnota bitu. Proto je velmi spolehlivý. Jediné číslo, které tento algoritmus nesprávně určí je 2, kvůli tomuto jedninému případu je tedy v programu daná výjimka.

Další funkcí je nsd_moderni_euklid, jejímž vstupem jsou dvě intové hodnoty a která spočítá největšího spoečného dělitele zadaných čísel a výstupe je tedy také intová proměnná. Algoritmus využitý v tomto případě je, jak již napovídá název, euklidův. Tato funkce je nejrychlejší z těch, které jsou v tomto souboru.

Další z funkcí počítající největší společný násobek je nsd_rozsireny_euklid. Vstupem jsou také dvě intové proměnné a výstupem pouze jedna. Algoritmem je rozšířený euklidův. Ve srovnání s nsd_moderni_euklid je asi třikrát pomalejší.

Poslední z funkcí počítající největší společný násobek je nsd_dvojkovy. Vsupem jsou také dvě intové proměnné a výstupem pouze jedna. Tato funkce využívá Steinův algoritmus. Z těchto tří funkcí je však nejpomalejší. Je totiž asi šesttkrát pomalejší než první z funkcí (nsd_moderni_euklid).

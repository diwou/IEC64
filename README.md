# IEC64W – IEEE-488-Interface für Commodore C64 & C128

![](https://codeberg.org/diwou/IEC64/raw/branch/main/Images/IEC64W_Interface.jpg)

## Einführung

Dies ist der Nachbau der IEC64-Karte aus den 1980er Jahren. Sie stellt eine GPIB- (IEEE-488-) Schnittstelle bereit und wird am Expansionsport des Commodore C64 oder C128 betrieben.

Wer der ursprüngliche Entwickler der Karte war, ließ sich nicht herausfinden. Sie wurde von „WAW Elektronik“, „Jann Datentechnik“ und „REX Datentechnik“ in unterschiedlichen Varianten vertrieben – die technische Grundlage und das Kernal waren jedoch immer identisch. Nur die Einschaltmeldung wurde jeweils an die entsprechende Firma angepasst.

Dies ist die Version, die damals von „WAW Elektronik“ verkauft wurde.

# Technik

Die Karte basiert auf dem MC6821P Peripheral Interface Adapter von Motorola. Außerdem ist das passende Kernal direkt als EPROM auf der Karte integriert.

Somit kann die Karte einfach eingesteckt und sofort genutzt werden. Das Kernal sowie die gesamte Karte lassen sich per DIP-Schalter deaktivieren. Ersteres ist insbesondere dann interessant, wenn man das Kernal intern im Rechner betreiben möchte.

Die Karte lässt sich so konfigurieren, dass ein Mischbetrieb aus IEC (z. B. 1541) und IEEE-488 möglich ist.

# Stückliste

Die Stückliste ist überschaubar. Der MC6821P ist gut über eBay oder UTSource erhältlich. Die genannten Hersteller dienen als Beispiele – selbstverständlich können auch Vergleichstypen anderer Hersteller verwendet werden.

| Menge | Bezeichnung   | Hersteller           | Herstellernummer             | Beschreibung |
|-------|----------------|----------------------|-------------------------------|--------------|
| 4     | C1–C4          | Dersonic             | CC1H104ZA1PD3F5O3000          | Keramik-Kondensator 100 nF, -20 % bis +80 %, 50 V, THT, Rastermaß 2,54 mm |
| 1     | J2             | L-Com                | CIB24SRA                      | GPIB-Steckverbinder, 90°, Buchse |
| 2     | R1, R2         | Yageo                | CFR-25JB-52-1K                | Widerstand 1 kΩ, 0,25 W, 5 %, axial |
| 1     | RN2            | Vishay Dale          | CSC06A0110K0GPA               | Widerstandsnetzwerk, 5 × 10 kΩ, 6-polig, SIP |
| 1     | RN1            | Vishay Dale          | CSC05A0110K0GPA               | Widerstandsnetzwerk, 4 × 10 kΩ, 5-polig, SIP |
| 1     | SW1 & SW2      | Würth Elektronik     | 418117270906                  | DIP-Schalter, 6-polig, 2,54 mm Raster, 24 V |
| 1     | U4             | Spansion             | AM27C128-150DC                | EPROM, UV, 128KBit, 16K × 8, 150 ns, 28-Pin CDIP |
| 1     | U2             | Texas Instruments    | SN74LS11N                     | AND-Gatter, 3-fach, 3 Eingänge, DIP-14 |
| 1     | U1             | Texas Instruments    | SN74LS00N                     | NAND-Gatter, 4-fach, DIP-14, 5,25 V |
| 1     | U3             | Motorola             | MC6821P                       | Peripheral Interface Adapter (PIA) |

# Lizenz

Der Inhalt dieses Repositories, mit Ausnahme der Verzeichnisse „Docs“ und „Software“, steht unter folgender Lizenz:

- **Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License (CC BY-NC-SA 4.0)**  
Der vollständige Lizenztext befindet sich in der Datei [LICENSE.CC-NC-BY-SA-4.0](https://codeberg.org/diwou/IEC64/Images/raw/branch/main/LICENSE.CC-NC-BY-SA)  
Eine Kopie ist außerdem hier verfügbar: https://creativecommons.org/licenses/by-nc-sa/4.0/

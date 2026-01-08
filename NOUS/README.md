# OŽIVENIE RELÉ NOUS L6T v TASMOTA systéme

Návod na konfiguráciu a kalibráciu NOUS L6T relé v systéme Tasmota.

## A - Nastavenie počtu desatinných miest

Zadaj v konzole postupne tieto príkazy:

```
VoltRes 3
WattRes 3
AmpRes 3
FrequencyRes 3
EnergyRes 5
CalcRes 5
```

Po zadaní príkazov vykonaj reštart:
```
RESTART 1
```

## B - Základná konfigurácia

Zadaj v konzole tieto príkazy:

| Príkaz | Popis |
|--------|-------|
| `IPAddress1 XXX.XXX.XXX.XXX` | Zadaj statickú IP adresu (nie je povinné) |
| `SetOption53 1` | Zobrazí IP adresu v MAIN MENU |
| `TelePeriod 60` | Každých 60 sekúnd odozva do MQTT (rozsah 30-3600) |

Po zadaní príkazov vykonaj reštart:
```
RESTART 1
```

## C - Kalibrácia napätia

**DÔLEŽITÉ: Modul sa dodáva NENAKALIBROVANÝ!**

1. Zmeraj meracím prístrojom napätie siete vo Voltoch
2. Zadaj kalibračný príkaz:

```
VoltageSet YYY,YY
```

Kde `YYY,YY` je namerané napätie (napr. `230,50`).

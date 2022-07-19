# AxAutoUpdate v1.0.6
## Opis
Skrypt pozwala na zarządzanie aktualizacjami skryptów (automatyczna aktualizacja)
## Informacje
### Komendy
- /update
  - list - wyswietla skrypty z mozliwoscia aktualizacji
  - on {script} - wlacza automatyczne aktualizowanie skryptu
  - off {script} - wylacza automatyczne aktualizowanie skryptu
  - version {script} - wyswietla aktualna wersje podanego skryptu
  - update {all/script} - aktualizuje wszystkie lub podany skrypt
  - unregister {script} - usuwa skrypt z listy automatycznych aktualizacji
### Działanie
- Jeżeli chcesz aby twój skrypt był automatycznie aktualizowany za pomoca AxAutoUpdate wklej te linijki na góre swojego skryptu
```
on load:
    set {AxUpdate::<nazwa>::link} to "<link>"
    set {AxUpdate::<nazwa>::status} to true
    set {AxUpdate::<nazwa>::name} to "<nazwa>"
    set {AxUpdate::<nazwa>} to script
```
- Albo jeżeli masz pewność że skrypt AxAutoUpdate jest zainstalowany na serwerze użyj funkcji
```
on load:
    AxUpdate_register("AxUpdate", "https://code.skript.pl/0uFoPX6y/raw", script)
```
## Instalacja
### Wymagania
- SkUtilities 0.9.2
### Instalacja
- Pobierz plugin Skript i wymagane pluginy
- Wrzuc plik do folderu plugins/Skript/scripts
- Przeładuj plik /sk reload {nazwa pliku}
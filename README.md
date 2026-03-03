# Projekt analizy danych pandemii COVID-19 oraz budowy modelu predykcyjnego

Projekt analizy danych pandemicznych obejmujący eksploracyjną analizę danych, interaktywną wizualizację oraz budowę modelu predykcyjnego.
Dane pochodzą z repozytorium WHO (World Health Organization) i dotyczą okresu pandemii COVID-19.

Projekt został zrealizowany w środowisku Python (analiza i modelowanie) oraz Tableau (wizualizacja).


## Cel projektu

Celem projektu jest:
- przygotowanie i oczyszczenie rzeczywistych, niejednorodnych danych pandemicznych,
- przeprowadzenie eksploracyjnej analizy danych (EDA),
- stworzenie interaktywnych dashboardów do analizy globalnej i krajowej,
- budowa oraz ewaluacja modeli uczenia maszynowego służących do predykcji wzrostów liczby zgonów.

Projekt obejmuje pełny pipeline analityczny – od surowych danych po wytrenowany model predykcyjny.


## Struktura projektu
- data/covid-data.csv
- Covid_analysis.ipynb
- Covid_analysis_viz.twbx
- Model.ipynb
- README.md


## Etapy projektu
### 1. Eksploracyjna analiza danych

Plik: Covid_analysis.ipynb

Notebook zawiera kompletny proces przygotowania danych:
- wczytanie danych,
- czyszczenie i obsługę braków,
- imputację,
- transformację i strukturyzację danych,
- analizę eksploracyjną (EDA).
Wynikiem końcowym jest przetworzony zbiór danych: covid-data-cleaned.csv


### 2. Interaktywna wizualizacja

Plik: Covid_analysis_viz.twbx

Plik zawiera dwa interaktywne dashboardy:
- Dashboard globalny – umożliwia analizę trendów pandemii na poziomie globalnym
- Dashboard krajowy – pozwala na szczegółową analizę wybranego kraju

Aby otworzyć plik:
- Zainstaluj darmową wersję Tableau Public
- Otwórz plik .twbx w programie

Dashboardy umożliwiają dynamiczną eksplorację danych oraz analizę zależności pomiędzy kluczowymi wskaźnikami.


### 3. Model predykcyjny

Plik: Model.ipynb

Notebook obejmuje:
- przygotowanie danych do modelowania,
- podział na zbiór treningowy i testowy,
- budowę modeli klasyfikacyjnych,
- ewaluację (precision, recall, F1-score, confusion matrix),
- optymalizację hiperparametrów.

Model, który osiągnął najlepsze wyniki, został zapisany do pliku .pkl, co umożliwia jego ponowne wykorzystanie bez potrzeby ponownego trenowania (ze względu na rozmiar model znajduje się w best_rf.zip).
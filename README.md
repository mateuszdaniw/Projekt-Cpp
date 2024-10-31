# Cenownik - Aplikacja monitorująca ceny produktów

Cenownik to aplikacja napisana w C++ z interfejsem graficznym Qt, służąca do monitorowania cen produktów na platformie Allegro. Aplikacja pozwala użytkownikom śledzić zmiany cen, wizualizować je na wykresach oraz ustawiać powiadomienia o okazjach cenowych. Dane są pobierane za pomocą libcurl, a następnie zapisywane w bazie danych PostgreSQL w celu ich analizy.

## Funkcjonalności

- **Monitorowanie cen produktów** – aplikacja pobiera dane o cenach produktów z API Allegro lub scrapuje dane bezpośrednio ze strony.
- **Wizualizacja zmian cen** – wykresy przedstawiające historię cen produktów w czasie (QtCharts).
- **Powiadomienia o okazjach** – użytkownik może ustawić alerty, które powiadomią go, gdy cena spadnie poniżej określonego poziomu.
- **Baza danych** – aplikacja zapisuje dane o produktach i ich cenach w bazie danych PostgreSQL, co umożliwia śledzenie historii zmian cen.
- **Interfejs graficzny** – przejrzysty i intuicyjny interfejs stworzony z użyciem Qt.

## Technologie

- **C++** – główny język programowania aplikacji.
- **Qt** – framework użyty do stworzenia interfejsu graficznego oraz wykresów.
- **libcurl** – biblioteka odpowiedzialna za pobieranie danych z sieci (API lub scrapowanie).
- **PostgreSQL** – baza danych używana do przechowywania historii cen produktów.
- **QtCharts** – moduł do generowania wykresów zmian cen w czasie.

## Instalacja

### Wymagania systemowe

- **C++ Compiler** – np. GCC lub MSVC.
- **Qt** – wersja 5.12 lub nowsza.
- **libcurl** – wersja 7.0 lub nowsza.
- **PostgreSQL** – baza danych do zapisywania danych o produktach i cenach.

### Kroki instalacji

1. **Klonowanie repozytorium**

   ```bash
   git clone https://github.com/mateuszdaniw/cenownik.git
   cd cenownik

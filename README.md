# Porsche Retirement Widget v6

Widget Android z przezroczystym zestawem zegarów i odliczaniem do 07.11.2028.

## Zmiany v6
- Dwie dostarczone przez użytkownika bitmapy 1774 × 887 px z kanałem alfa: `cluster_40.png` i `cluster_60.png`.
- Lewa wskazówka jest częścią bitmapy, nie jest już dorysowywana w kodzie.
- Bitmapa i wyświetlacz seksapilu przełączają się razem co dzień między 40% i 60%.
- Środkowa wskazówka i licznik dni zachowują działanie z v5.
- Wersja APK: 6.0 (`versionCode` 6).

## GitHub Actions
Workflow `.github/workflows/build.yml` uruchamia się po push na `main` i ręcznie. Po zielonym wyniku otwórz run i pobierz artifact `Porsche-Retirement-v6-APK`; wewnątrz znajduje się `app-debug.apk`.

## Instalacja
Zainstaluj APK na telefonie. Ponieważ `applicationId` jest taki sam jak w v5, aktualizacja powinna działać, jeśli podpis debug APK jest zgodny. Na różnych maszynach GitHub Actions klucz debug może się zmienić i Android odmówi aktualizacji — wtedy odinstaluj v5 i zainstaluj v6, a następnie dodaj widget ponownie.

## Testowanie
Zmiana daty telefonu pozwala sprawdzić środkową wskazówkę i naprzemienność 40/60. Po testach przywróć automatyczną datę i godzinę.

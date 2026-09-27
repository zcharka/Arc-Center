# Arc Center

## EN
Arc Center is a modular, dynamic widget loader application built with Python, GTK4, and Libadwaita. It serves as a centralized hub (control center) that dynamically loads, displays, and manages system utility widgets from a specific directory.

Designed to be the core interface for the Arc OS/Tooling ecosystem, it features a robust localization system, safety locking for subprocesses, and a responsive user interface that respects GNOME system settings.

### Key Features

- **Dynamic Widget Loading:** Automatically discovers and loads Python-based widgets from `/usr/share/arcos/widgets`.
- **Modern UI:** Built with GTK4 and Libadwaita for a native GNOME look and feel, featuring a responsive sidebar and split-view layout.
- **Robust Localization (L10n):** Custom localization engine that supports per-widget translation dictionaries, recursive pattern matching (e.g., handling variables inside translated strings), and dynamic text updates.
- **Safety Locking:** Automatically locks the UI and window controls when a widget executes a subprocess (via monkey-patched `subprocess` calls) to prevent user interference during critical operations.
- **Single Widget Mode:** Can be launched via command line to display a specific widget in a standalone window without the sidebar.
- **System Integration:** Respects system button layouts (close/minimize/maximize placement) and follows system dark/light mode preferences.

### Dependencies:
- Python 3.8+
- GTK 4
- Libadwaita
- PyGObject

## PL
Arc Center to modułowa, dynamiczna aplikacja do ładowania widżetów, stworzona w Pythonie z wykorzystaniem GTK4 i Libadwaita. Służy jako scentralizowane centrum (centrum sterowania), które dynamicznie ładuje, wyświetla i zarządza widżetami narzędzi systemowych z określonego katalogu.

Zaprojektowana jako główny interfejs ekosystemu Arc OS/Tooling, oferuje rozbudowany system lokalizacji, mechanizm blokady bezpieczeństwa dla procesów podrzędnych oraz responsywny interfejs użytkownika, który respektuje ustawienia systemowe GNOME.

### Główne funkcje

* **Dynamiczne ładowanie widżetów:** Automatycznie wykrywa i ładuje widżety napisane w Pythonie z katalogu `/usr/share/arcos/widgets`.
* **Nowoczesny interfejs:** Zbudowany przy użyciu GTK4 i Libadwaita, zapewnia natywny wygląd i działanie w środowisku GNOME, wraz z responsywnym paskiem bocznym i układem podzielonego widoku.
* **Rozbudowany system lokalizacji (L10n):** Własny mechanizm lokalizacji obsługujący osobne słowniki tłumaczeń dla każdego widżetu, rekurencyjne wyszukiwanie wzorców (np. obsługę zmiennych wewnątrz przetłumaczonych tekstów) oraz dynamiczną aktualizację tekstów.
* **Blokada bezpieczeństwa:** Automatycznie blokuje interfejs użytkownika i elementy sterujące oknem, gdy widżet uruchamia proces podrzędny (za pomocą zmodyfikowanych wywołań `subprocess`), aby zapobiec ingerencji użytkownika podczas wykonywania krytycznych operacji.
* **Tryb pojedynczego widżetu:** Może zostać uruchomiony z poziomu wiersza poleceń w celu wyświetlenia konkretnego widżetu w osobnym oknie, bez paska bocznego.
* **Integracja z systemem:** Respektuje systemowe ustawienia rozmieszczenia przycisków okna (zamykanie/minimalizacja/maksymalizacja) oraz dostosowuje się do ustawień trybu jasnego/ciemnego systemu.

### Zależności

* Python 3.8+
* GTK 4
* Libadwaita
* PyGObject

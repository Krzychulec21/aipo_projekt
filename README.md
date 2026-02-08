# Projekt Detekcji Upadków (Fall Detection)

Ten projekt wykorzystuje architekturę sieci głębokich łączącą **ResNet50** (jako ekstraktor cech wizualnych) oraz sieć **LSTM** (do analizy sekwencji czasowej) w celu klasyfikacji zdarzeń jako upadek (FALL) lub codzienna czynność (ADL).

## Struktura projektu

Projekt opiera się na zbiorze danych [UR Fall Detection Dataset](https://fenix.ur.edu.pl/mkepski/ds/uf.html). Aby skrypt działał poprawnie, dane muszą być umieszczone w folderze `data` zgodnie z poniższym schematem:

```text
projekt/
├── main.ipynb          # Główny plik z modelem i procesem uczenia
├── requirements.txt    # Lista bibliotek niezbędnych do uruchomienia
├── data/
│   ├── adl/            # Podfoldery z klatkami .png dla czynności codziennych
│   └── fall/           # Podfoldery z klatkami .png dla upadków
└── ...

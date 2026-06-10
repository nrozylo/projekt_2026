# Przewidywanie zużycia energii w budynkach 

## Opis projektu:
Głównym celem projektu jest zbudowanie dwóch modeli predykcyjnych korzystając `train_energy_data.scv`, które na podstawie danych takich jak metraż, liczba osób w budynku oraz liczba urządzeń elektrycznych, są w stanie przewidzieć ilość zużytej energii w danym budynku (jednostka = kWh).

## Zawartość repozytorium:
- notatnik `projekt_energy.ipnyb` w Google Colab. Zawiera on:
  - eksplorację i wizualizację danych,
  - czyszczenie danych oraz zbudowanie Pipeline,
  - implementację modeli Linear Regression i Random Forest Regressor, wraz z optymalizacją hiperparametrów,
  - porównanie modeli i wskazanie lepszego.
- zbiór danych `train_energy_data.csv`

## Kroki podjęte w projekcie:
1. Analiza danych i wizualizacja - ukazanie struktury oraz danych statystycznych, histogramy (rozkład parametrów), macierz korelacji.
2. Czyszczenie i przygotowanie danych - zastosowano kod wykrywający i usuwający duplikaty oraz outliery, podzielono dane przy użyciu `train_test_split`, stworzono potok, aby przygotować stabilny model.
3. Uczenie maszynowe - zbudowano modele Linear Regression, Random Forest, oraz Random Forest z zastosowaniem `GridSearchCV`.
4. Porównanie modeli i wskazanie najlepszego z nich.

## Wyniki:
- **Najlepszy model**: Linear Regression
- **Wskaźnik RMSE**: 0.0137
- **Optymalne parametry dla Random Forest**: `{'max_depth': 20, 'min_samples_split': 2, 'n_estimators': 150}`




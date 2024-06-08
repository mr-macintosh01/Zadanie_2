# Zadanie_2

# Test CI Docker Scout

To repozytorium zawiera konfigurację workflow GitHub Actions do testowania obrazów Docker pod kątem wysokich i krytycznych podatności za pomocą Docker Scout.

## Konfiguracja

Workflow CI jest zdefiniowany w pliku `.github/workflows/ci.yaml`. Składa się z dwóch zadań:
- `Docker Scout Analysis for High Vulnerabilities`: Testuje obraz Docker pod kątem wysokich podatności.
- `Docker Scout Analysis for Critical Vulnerabilities`: Testuje obraz Docker pod kątem krytycznych podatności.

Każde zadanie uruchamia narzędzie wiersza poleceń Docker Scout, aby przeanalizować obraz Docker określony przez repozytorium i SHA commita.

## Użycie

1. Upewnij się, że Docker Scout jest poprawnie skonfigurowany w tajnych zmiennych repozytorium GitHub.
2. Wprowadź zmiany do swojego repozytorium, aby uruchomić workflow CI.
3. Sprawdź wyniki workflow na karcie GitHub Actions swojego repozytorium, aby sprawdzić, czy znaleziono jakieś wysokie lub krytyczne podatności.

## Przykładowe wyniki

Po uruchomieniu workflow, wyniki wskażą, czy znaleziono jakieś wysokie lub krytyczne podatności w obrazie Docker.

```plaintext
...
No high vulnerabilities found.
...

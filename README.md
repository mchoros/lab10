# Laboratorium

GitHub Actions - przeglad podstawowych rozwiazan

1. Uzupełnienie pliku gha_example.yml

2. Operacje z gitem: 
    - Commit: 
        git add . && git commit -m "GA test run"

    - Pushowanie do repo:
        git push

    - Wyświetlenie listy workflow:
        gh workflow list
    
    - Uruchomienie workflow:
        gh workflow run 57738285

3. Sprawdzenie poprawności funkcjonowania workflow:
        gh run list --workflow=gha_example.yml

        gh run view 5026769191

        gh run view --job=13616118010

4. Screen z potwierdzenia działania znajduje się załączony do repo

Budowanie przebiegło pomyślnie przed podłączeniem dockerhuba do repo.
Po podłączeniu pomyślnie loguje, ale przy budowaniu występuje błąd autoryzacji, a co za tym idzie nie mogę wrzucić obrazów na dockerhuba.
Token z dockerhuba został wygenerowany z pełnymi uprawnieniami, w sposób pokazany w skrypcie z zajęć.
Logowanie do dockera przebiegło poleceniem pokazanym w skrypcie za pomocą tokena
Nazwy tokenów są takie same jak te w plikach .yml, dla potwierdzenia dołączam screeny do repo.

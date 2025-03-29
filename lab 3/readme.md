### Użytkownicy
- Rozbuduj model użytkownika o rolę. Możliwe role: admin, devops, developer.
- Zamockuj listę użytkowników. Zalogowany pozostaje admin, na liście powinien być jeszcze minimum jeden developer i jeden devops  
### Zadania
Zadanie to najmniejsza jednostka projektu. Jest wykonywana przez jedną osobę, jest przypisane do konkretnej historyjki, jest możliwe do zamknięcia. 
- Zrealizuj CRUD do zadania. 
- Zrealizuj widok szczegółów zadania - dane zadania, przypisana historyjka, data startu, zrealizowane roboczogodziny, przypisana osoba 
- Widok szczegółów zadania (lub dodatkowy widok) powinien dostarczać możliwość przypisania osoby do zadania (devops lub developer). Przypisanie osoby automatycznie zmienia stan zadania z "todo" na "doing" oraz uzupełnia datę startu zadania.
- Widok szczegółów zadania (lub dodatkowy widok) powinien dostarczać możliwość zmiany stanu zadania na "done". Zmiana stanu automatycznie uzupełnia datę zakończenia zadania.
- Zrealizuj widok tablicy kanban z zadaniami (kolumny todo, doing, done)
- Zadania powinny się zapisywać za pośrednictwem mechanizmu komunikacji z api


Model Zadania: 
- Nazwa
- Opis
- Priorytet (niski/średni/wysoki)
- Historyjka do której przynależy zadanie
- Przewidywany czas wykonania
- Stan (todo, doing, done). Zadanie ze stanem doing musi posiadać czas startu oraz przypisanego użytkownika. Zadanie ze stanem done posiada przypisanego użytkownika oraz datę zakończenia
- Data dodania
- Data startu (stan zmieniony na doing)
- Data zakończenia (stan zmieniony na done)
- Użytkownik odpowiedzialny za zadanie (zadanie może wykonywać devops lub developer)


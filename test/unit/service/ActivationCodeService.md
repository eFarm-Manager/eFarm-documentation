1. sprawdza poprawny kod
2. sprawdza nieprawidlowy kod
3. sprawdza wygasniety kod
4. sprawdza zuzyty kod
5. poprawnie uzywa kod
6. RuntimeException jezeli proba uzycia kodu ktory nie istnieje
7. owner przy logowaniu dostaje informacje o tym za ile dni wygasnie kod
8. brak info jak >14 dni do wygasniecia
9. manager czyli nie owner nie ma informacji
10. znajduje kod aktywacyjny przez farm id
11. nie znajduje kodu aktywacyjnego przez farm id
12. znajduje kod aktywacujny poprzez swoje id
13. nie znajduje nieistnejacego kodu poprzez swoje id
14. powinno zmienic kod aktywacyjny
15. jezeli cos nie tak z kodem np. zuzyty to wylapuje bad request
16. blokuje uzytkownika jezeli za duzo prob logowania ze zmienionym kodem aktywacyjnym

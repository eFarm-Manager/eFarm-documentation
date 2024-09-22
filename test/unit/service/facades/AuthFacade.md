1. poprawnie autentykuje logowanie
2. zwraca bad request dla nie aktywnego usera
3. zle haslo podczas logowania
4. zwraca forbidden jezeli gospodarstwo nie aktywne
5. zwraca info dla onwera jezeli kod wygasnie niedlugo 0..<14
6. poprawnie tworzy nowego usera przez zwykly signup
7. zwraca errory z binding result
8. error jak login zajety
9. error jak gospodarstwo nie znalezione
10. poprawnie tworzy nowego usera oraz gospodarstwo
11. zwraca errory z binding result
12. error jak login zajety
13. error jak farm name zajety
14. bad request jak kod nie istnieje
15. bad request jak kod zuzyty
16. jezeli odznaczenie kodu aktywacyjnego nie zadziala poprawnie to bad request
17. poprawnie robi aktualizacje kodu aktywacyjnego dla ownera
18. jezeli nie onwer to brak uprawnien
19. zwraca bad request jezeli update sie nie uda

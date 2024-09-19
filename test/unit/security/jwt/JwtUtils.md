1. zwraca jwt jezeli cookie istnieje - getJwtFromCookie
2. zwraca null jezeli cookie nie istnieje - getJwtFromCookie
3. jezeli request jest null to wtedy IllegalArgumentException - getJwtFromCookie
4. sprawdza poprawnosc tokenu wytworzonego - generateJwtCookie
5. jezeli brak user details to NullPointerException - generateJwtCookie
6. cookies roznia sie - generateJwtCookie
7. zwraca czysty token - getCleanJwtCookie
8. zwraca uzytkownika z valid token - getUserNameFromJwtToken
9. jezeli token expired to ExpiredJwtException - getUserNameFromJwtToken
10. jezeli token malformed to MalformedJwtException - getUserNameFromJwtToken
11. jezeli token empty to IllegalArgumentException - getUserNameFromJwtToken
12. poprawnie waliduje poprawny token - validateJwtToken
13. zwraca false dla expired token - validateJwtToken
14. zwraca false dla malformed token - validateJwtToken
15. zwraca false dla unsupported token - validateJwtToken
16. zwraca false dla empty token - validateJwtToken

# api_service

Zadanie jest następujące: Napisać kod klasy BaseService do komunikacji z restApi, z której będą mogły dziedziczyć serwisy używane w aplikacji. Klasa dziedzicząca powinna implementować jedynie metodę `call()`.  Przykładowo przy użyciu https://jsonplaceholder.typicode.com/ klasa potomna CreatePost powinna przyjmowac jako paramtr post (strukture, hash lub obiekt - pełna dowolnośc), natomiast jej wynikiem powinno byc wykonania requestu `POST /posts` i utworzenie odpowiadajacego zasobu w zewnetrznym api.

## Klasa bazowa powinna:
- obsługiwać błędy w odpowiedziach od Api
- zapewniać interfejs dostępu do odpowiedzi serwera
- wymuszać implementację metody `call()` w klasach potomnych
- udostępniać intefejs do stwierdzenia czy operacja zakonczyła się suckesem lub błędem
- maksymalnie ułatwiać implementację konkretnych serwisów
- wymuszać możliwie najlepsze praktyki podczas korzystania z niej
## Klasa bazowa nie musi:
- implementowac logiki zapytań HTTP, można użyć gotowej biblioteki jak [Faraday](https://github.com/lostisland/faraday)
- implementować parsowania JSON, można użyć zewnętrznej biblioteki
- wykonywać żadnych operacji na danych, takich jak zapisywanie ich do bazy danych lub pliku
- nie musi działać w środowisku Ruby on Rails, może być napisana w "czystym rubym"

Zadanie ma przede wszytskim pokazać zdolność do programowania w ruby zatem mile widziane będzie wykorzystanie możliwie największej ilości featerów języka i rozwiązywanie problemów `in ruby way`

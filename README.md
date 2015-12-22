В адаптере (GuzzleAdapter) есть возможность переключения тестового и боевого окружений.
Это осуществляется с помощью флага test (true - тестовое, false - боевое), который передается в конструктор GuzzleAdapter третьим параметром.
По умолчанию значение флага test - true, т.е. тестовое окружение.
Тестовое окружение - все запросы идут на тестовый урл http://api.dev.apiship.ru/v1/.
Боевое окружение - все запросы идут на боевой урл https://api.apiship.ru/v1/.
В адаптере (GuzzleAdapter) есть метод isTest, с помощью которого можно определить, какое окружение развернуто (тестовое или боевое).
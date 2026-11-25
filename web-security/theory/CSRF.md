# CSRF (Cross-Site Request Forgery)

CSRF — уязвимость, при которой сторонняя страница инициирует запрос через браузер пользователя. Браузер отправляет этот запрос на сервер веб-приложения, а веб-приложение выполняет нежелательное действие в активной сессии пользователя.

**Противодействие** — CSRF-токен и атрибут `SameSite` для cookie сессии. Сервер проверяет токен перед выполнением защищаемого действия. Значения `SameSite=Lax` и `SameSite=Strict` ограничивают отправку cookie в запросах с другого сайта. [OWASP — защита от CSRF](https://cheatsheetseries.owasp.org/cheatsheets/Cross-Site_Request_Forgery_Prevention_Cheat_Sheet.html)

[Различие между CSRF и SSRF](CSRF_VS_SSRF.md)

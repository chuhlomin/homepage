---
date: 2020-08-10
---

# Webmention

В 2017 году была опубликована спецификация Webmention. Это такой «простой» способ уведомить один сайт, что на какую-то страницу ссылается другой сайт.

https://webmention.net/draft/

Например, Боб в своем блоге пишет статью, ссылаясь на статью в блоге Алисы. Движок блога, который использует Боб, отправляет запрос на страницу поста Алисы в поисках ссылки на сервис Webmention (где-то в заголовках или теле странице). Если такая ссылка найдена, то следом отправляется POST-запрос с указанием ссылок на оба блог-поста. Движок блога Алисы «регистрирует» это уведомление, опционально уведомляя «Боба» по какой ссылке можно проверять статус обработки webmention.

![Webmention sequence diagrams](webmention.png "Webmention sequence diagrams")

Всё это вытекает из идей децентрализованного интернета:  
https://indieweb.org/federation

Примеры реализций:  
https://indieweb.org/Webmention#IndieWeb_Examples

#rfc
# Тестовое задание на позицию .Net backend developer

Необходимо спроектировать и разработать приложение для анализа изменений содержимого сайтов.

## Сценарий использования

Конечный пользователь передаёт в приложение адрес веб-страницы, за которой следует наблюдать. Спустя произвольное время в рамках повторного обращения он получает список изменений, а затем актуальное содержимое страницы на интересующий его момент.

## Постановка задачи

Требуется написать сервер приложения. Он должен предоставлять публичный API, позволяющий выполнять как минимум следующие действия:
  - передача url страницы, за которой следует вести наблюдение;
  - получение списка изменений по заданному url;
  - получение деталей конкретного изменения.
  
При поступлении в систему нового url, за ним должно начинаться наблюдение. Изменением считается любое отличие html-разметки страницы от сохранённой ранее. При выполнении задания следует учитывать изменения только в рамках указанной страницы, не нужно анализировать граф всего сайта.

Сервер не должен терять данные при перезапуске и в случае аварийного завершения работы, не должен падать при получении некорректных запросов.

## Требования к решению

Работа должна быть выполнена на языке C#. Допускаются зависимости от сторонних nuget-модулей. Для хранения данных можно использовать как собственное решение, так и любую существующую базу данных. Прочие технические решения (такие как, например, выбор версии фреймворка, модели хостинга, транспортного протокола и формата сообщений) остаются на усмотрение разработчика.

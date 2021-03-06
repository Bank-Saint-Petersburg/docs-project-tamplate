# API спецификация проекта

В данном разделе находится документация описывающая API endpoints и модели.
Для описания используются OpenAPI Specification и AsyncAPI Specification.

## Endpoints

В разделе `api/reference` находится описание `endpoints` с форматами обращения к ним. Это могут быть как REST API так и асинхронное API типа WebSocket или каналов для очередей.

Здесь могут встречаться вложенные модели, но если требуется использование базовых сущностей, то описание модели этих сущностей должно быть вынесено в раздел `api/models`. Это следует делать для наглядности и возможности ссылаться на эти модели в других проектах.

Перед созданием нового API убедитесь что в данном проекте ещё нет похожего API.

Старайтесь работать с единым файлом и добавлять все новые `endpoints` в него.

## Модели

В разделе `api/models` находится описание моделей для основных сущностей используемых в API проекта. 
На каждую модель заводится отдельный YAML файл с названием данной сущности и версией `EntityName.v1.yaml`. Stoplight из коробки умеет формировать правильное название модели если создавать его через `Add` -> `Model`.

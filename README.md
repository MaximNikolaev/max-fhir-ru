# Что и зачем

Собственная реализация FHIR Implementation Guide для России, написанная на энтузиазме по данным
сайта [fhir.ru](http://fhir-ru.zendoc.me/)

Одна из основных задач - генерировать полный набор файлов спецификации FHIR IG с выполнением валидации xml/json
файлов

Элементы спецификации не создаются с нуля, а всегда наследуются от базовых
ресурсов [http://hl7.org/fhir/](http://hl7.org/fhir/) через тег `baseDefinition`

При сборке отслеживаеся качество на странице [qa.html](https://maximnikolaev.github.io/max-fhir-ru/qa.html)

[GitHub Pages](https://maximnikolaev.github.io/max-fhir-ru/)

[Репозиторий](https://github.com/MaximNikolaev/max-fhir-ru)

# Особенности

- На данный момент конечный результат (этот проект) собирается вручную, без CI-инструментов
- Собран на базе репозитория `FHIR/sample-ig:master`
- Использует шаблон версии `0.2.2` из http://fhir.org/templates/fhir.base.template/history.html
- В репозиторий вручную выкладывается содержимое папки `/output` после
  работы [IG Publisher](https://github.com/HL7/fhir-ig-publisher/releases/latest/download/publisher.jar)-а
- При каждой сборке проект полностью перезаписывается

# TODO

- Для переводов наименований и описаний на русский язык не использовать тег `differential`, а применять механизм
  тега `language`
- Заменить `uv` на `ru` в идентификаторе проекта `hl7.fhir.uv.max-fhir-ru`
- Заменить `constraint` на `specialization` в тегах `derivation`
  (сейчас при указании specialization при сборке формируются пустые файлы схематронов sch)

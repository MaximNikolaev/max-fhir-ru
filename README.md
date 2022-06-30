# Что здесь

Собственная реализация FHIR Implementation Guide для России, написанная на энтузиазме по данным
проекта [fhir.ru](http://fhir-ru.zendoc.me/)


[GitHub Pages](https://maximnikolaev.github.io/max-fhir-ru/)

[Репозиторий](https://github.com/MaximNikolaev/max-fhir-ru)

# Особенности

- На данный момент конечный результат (этот проект) собирается вручную, без CI-инструментов
- Собран на базе репозитория `FHIR/sample-ig:master`
- Использует шаблон версии `0.2.2` из [http://fhir.org/templates/fhir.base.template/history.html]()
- В репозиторий вручную выкладывается содержимое папки `/output` после
  работы [IG Publisher](https://github.com/HL7/fhir-ig-publisher/releases/latest/download/publisher.jar)-а
- При каждой сборке проект полностью перезаписывается

# TODO

- Для переводов наименований и описаний на русский язык не использовать тег `differential`, а применять механизм
  тега `language`
- Заменить `uv` на `ru` в идентификаторе проекта `hl7.fhir.uv.max-fhir-ru`
- убрать rim-mapping для extension-ов
- для всех реквизитов, которые могут изменяться со времением, сделать структуры для хранения историй?
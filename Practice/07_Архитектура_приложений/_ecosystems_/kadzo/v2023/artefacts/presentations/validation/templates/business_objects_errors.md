# Ошибки "Бизнес-сущностей"

{{#general}}
## Базовые атрибуты
Ошибки в атрибуте "Наименование" и "Статус" (title, status)
![Загрузка ошибок](@entity/kadzo.v2023.business_objects/validation.base_attrib?domain={{domain}})
{{/general}}

{{#processes}}
## Ссылка на бизнес-процесс
Ошибки в атрибуте "Используется в бизнес-процессах" (processes)
![Загрузка ошибок](@entity/kadzo.v2023.business_objects/validation.process_attrib?domain={{domain}})
{{/processes}}

{{#data_objects}}
## Объекты данных
Бизнес-объекты без объектов данных.
![Загрузка ошибок](@entity/kadzo.v2023.business_objects/validation.data_objects?domain={{domain}})
{{/data_objects}}

{{^iserrors}}
**А где ошибки?** :O

Я тебя поздравляю, ты справился ;)  
Не, ну надо же...

С ума сойти...  
Ни одной ошибки.
{{/iserrors}}
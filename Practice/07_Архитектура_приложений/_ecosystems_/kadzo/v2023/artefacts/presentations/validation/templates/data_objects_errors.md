# Ошибки "Объектов данных"

{{#general}}
## Базовые атрибуты
Ошибки в атрибутах "Наименование", "Категория" и "Статус" (title, category, status)
![Загрузка ошибок](@entity/kadzo.v2023.data_objects/validation.base_attrib?domain={{domain}})
{{/general}}

{{#parent}}
## Родительская "Бизнес-сущность"
Ошибки в атрибуте "Родительский бизнес-объект" (business_object)
![Загрузка ошибок](@entity/kadzo.v2023.data_objects/validation.parent_attrib?domain={{domain}})
{{/parent}}

{{#master_system}}
## Мастер система
Ошибки в атрибуте "АС, являющаяся мастер системой для объекта данных" (master_system)
![Загрузка ошибок](@entity/kadzo.v2023.data_objects/validation.master_system_attrib?domain={{domain}})
{{/master_system}}

{{^iserrors}}
**У тебя нет ошибок, садись 5-ка!**

Ты на пути к **level 3** на тепловой карте :D


{{/iserrors}}
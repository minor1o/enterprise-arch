# Ошибки "Параметров ТА"

{{#general}}
## Базовые атрибуты
Ошибки в атрибутах "Тип компонента", "Прикладное ПО" и "Масштабируемость" (type, software, scalability)
![Загрузка ошибок базовых атрибутов](@entity/kadzo.v2023.tech_params/validation.base_attrib?domain={{domain}})
{{/general}}

{{#ha}}
## HA атрибуты
Ошибки в атрибутах HA
![Загрузка ошибок атрибутов HA](@entity/kadzo.v2023.tech_params/validation.ha_attrib?domain={{domain}})
{{/ha}}

{{#hac}}
## Консистентность HA атрибутов
Ошибки в комбинациях атрибутов HA
![Загрузка ошибок атрибутов HA](@entity/kadzo.v2023.tech_params/validation.ha_consistency?domain={{domain}})
{{/hac}}

{{#dr}}
## DR атрибуты
Ошибки в атрибутах DR
![Загрузка ошибок атрибутов DR](@entity/kadzo.v2023.tech_params/validation.dr_attrib?domain={{domain}})
{{/dr}}

{{#drc}}
## Консистентность DR атрибутов
Ошибки в комбинациях атрибутов DR
![Загрузка ошибок атрибутов DR](@entity/kadzo.v2023.tech_params/validation.dr_consistency?domain={{domain}})
{{/drc}}

{{#system}}
## Атрибут Система
Ошибки в атрибутe "Система" (system)
![Системы](@entity/kadzo.v2023.tech_params/validation.system_attrib?domain={{domain}})
{{/system}}

{{#monitoring}}
## Мониторинг
Все компоненты должны быть подключены к мониторингу
![OMG](@entity/kadzo.v2023.tech_params/validation.monitoring_attrib?domain={{domain}})
{{/monitoring}}

{{#backup}}
## Резервное копирование
Если отсутствует, то должно быть "отсутствует" и в место хранения дубликата".
Если что угодно кроме отсутствует, должно быть указано место хранения копии
![OMG](@entity/kadzo.v2023.tech_params/validation.backup_attrib?domain={{domain}})
{{/backup}}

{{#crreq}}
## Выполнение требований для уровня критичности
Для всех компонент, относящихся к системам уровня BC\MC, параметры отказоустойчивости и катастрофоустойчивости должны принимать значения: type = "Да", "Тип резервирования мощностей и данных" = "Полное", "Полнота резервирования мощностей и данных" = "Полное".
![OMG](@entity/kadzo.v2023.tech_params/validation.crreq?domain={{domain}})
{{/crreq}}


{{^iserrors}}
**Считайте вы прошли техническое собеседование в ДКА**

Да, чуть не забыли, проверьте, что в Технических сервисах у вас тоже порядок, потом ждем резюме.

Адреса нет? - Ты же технарь, адрес найдешь ;)

{{/iserrors}}
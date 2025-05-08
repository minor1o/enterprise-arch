# Ошибки "Клиентов"

{{#general}}
## Базовые атрибуты
Ошибки в атрибутах "Клиенты", "Тип клиентов" и "Количество" (title, type, count)
![Загрузка ошибок](@entity/kadzo.v2023.clients/validation.base_attrib?domain={{domain}})
{{/general}}

{{#client_channel}}
## Клиенты без связи с каналами
![Загрузка ошибок](@entity/kadzo.v2023.clients/validation.client_channel?domain={{domain}})
{{/client_channel}}

{{^iserrors}}
**С клиентами у вас никаких проблем, да?**

Ничего, посмотрим как вы справитесь на ассессменте :D

Шучу, шучу...

Или нет :scream:

{{/iserrors}}
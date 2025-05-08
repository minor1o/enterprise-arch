# Ошибки "Каналов взаимодействия с клиентом"

{{#general}}
## Базовые атрибуты
Ошибки в атрибуте "Наименование", "Описание" и "Статус" (title, description, status)
![Загрузка ошибок](@entity/kadzo.v2023.channels/validation.base_attrib?domain={{domain}})
{{/general}}

{{#products}}
## Ссылки на продукты
Ошибки в атрибуте "Продукты, поставляемые в канале" (products)
![Загрузка ошибок](@entity/kadzo.v2023.channels/validation.products_attrib?domain={{domain}})
{{/products}}

{{#clients}}
## Ссылки на клиентов
Ошибки в атрибуте "Клиенты" (clients)
![Загрузка ошибок](@entity/kadzo.v2023.channels/validation.clients_attrib?domain={{domain}})
{{/clients}}

{{#systems}}
## Ссылки на системы
Ошибки в атрибуте "Связи с АС" (systems)
![Загрузка ошибок](@entity/kadzo.v2023.channels/validation.systems_attrib?domain={{domain}})
{{/systems}}

{{^iserrors}}
**Так каналами управляет только ММТС М9**

Или там другие каналы?

Ладно, ладно, мы все равно в легком шоке от вашей профессиональности :)

{{/iserrors}}
{{#functionalities}}
## Наличие функциональностей
Для каждой системы в домене компании, указанной в реестре АС (Р11_АС/kadzo.v2023.systems), должна быть указана как минимум одна функциональность.
![Загрузка ошибок](@entity/kadzo.v2023.systems/validation.without_functions?domain={{domain}})
{{/functionalities}}

{{#data_objects}}
## Объекты данных
Бизнес-объекты без объектов данных.
![Загрузка ошибок](@entity/kadzo.v2023.business_objects/validation.data_objects?domain={{domain}})
{{/data_objects}}

{{#client_channel}}
## Клиенты без связи с каналами
![Загрузка ошибок](@entity/kadzo.v2023.clients/validation.client_channel?domain={{domain}})
{{/client_channel}}

{{#check}}
## Ошибок в реестре кросс-проверок нет
{{/check}}
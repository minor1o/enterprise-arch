# Канал {{title}}

## Карточка
|                                     |                 |
|:-----------------------------------:|:---------------:|
|          **Идентификатор**          |    *{{id}}*     |
|          **Наименование**           |    {{title}}    |
|            **Описание**             | {{description}} |
|           **Тип канала**            |    {{type}}     |
|       **Размещение/владение**       |  {{location}}   |
|             **Статус**              |   {{status}}    |
|    **Способы защиты канала**        |  {{security}}   |
|           **Комментарий**           |  {{comments}}   |


## АС, доступные через канал
![Системы](@entity/kadzo.v2023.systems/systems_by_channel?channel={{id}})

## Продукты, поставляемые в канале
![Продукты](@entity/kadzo.v2023.products/products_by_channel?channel={{id}})

## Клиенты, обслуживаемые в канале
![Клиенты](@entity/kadzo.v2023.clients/clients_by_channel?channel={{id}})
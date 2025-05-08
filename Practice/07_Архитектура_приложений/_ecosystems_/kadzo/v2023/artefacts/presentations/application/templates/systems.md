# Система {{title}}

## Карточка
|                                       |                                |
|:-------------------------------------:|:------------------------------:|
|           **Идентификатор**           |            *{{id}}*            |
|          **Родительская АС**          | [{{parent}}]({{parent_link}})  |
|             **Описание**              |        {{description}}         |
|        **Уровень критичности**        |     ==*{{criticality}}*==      |
|               **Класс**               |           {{class}}            |
|            **Размещение**             |          {{location}}          |
|         **Степень владения**          |         {{ownership}}          |
|     **Тип изменений**                 |     {{change-type}}            |
|       **Этап жизненного цикла**       |         {{live-stage}}         |
| **Этап жизненного цикла на горизонт** |     {{live-stage-target}}      |
|          **Целевой статус**           |           {{status}}           |
|        **Производительность**         |        {{performance}}         |
|             **RTO (час)**             |            {{rto}}             |
|             **RPO (час)**             |            {{rpo}}             |
|                **SLA**                |            {{sla}}             |
|            **Мониторинг**             |         {{monitoring}}         |

## Функции системы
![Функции системы](@entity/kadzo.v2023.functions/system_functions?system_id={{id}})

## Каналы взаимодействия с системой
![Каналы взаимодействия с системой](@entity/kadzo.v2023.channels/system_channels?system_id={{id}})

## Бизнес-процессы, обеспечивающиеся системой
![Бизнес_процессы_с_системой](@entity/kadzo.v2023.processes/processes_by_system?system_id={{id}})

## Мастер система для данных
![Мастер система для данных](@entity/kadzo.v2023.data_objects/system_data_objects?system_id={{id}})

## Контекст (текущий) 
![Контекст(as-is)](@entity/kadzo.v2023.system_context/system_context_asis?system={{id}})

## Контекст (целевой) 
![Контекст(to-be)](@entity/kadzo.v2023.system_context/system_context?system={{id}})

## Исходящие интеграционные потоки
![Исходящие потоки](@entity/kadzo.v2023.integrations/integrations_by_src?system_id={{id}})

## Входящие интеграционные потоки
![Входящие потоки](@entity/kadzo.v2023.integrations/integrations_by_consumer?system_id={{id}})

## Параметры ТА системы {{title}}
![Параметры ТА](@entity/kadzo.v2023.tech_params_by_systems/tech_params_by_systems?system_id={{id}})
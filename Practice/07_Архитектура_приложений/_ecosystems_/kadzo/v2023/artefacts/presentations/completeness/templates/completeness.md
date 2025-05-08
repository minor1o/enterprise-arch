## Оценка расчета полноты архитектуры {{total}}
## Оценка расчета полноты архитектуры с учетом исключений {{total_except}}
Информационная оценка полноты заполнения КА ДЗО.
Расчет полноты архитектуры строится на основе результатов работы валидаторов.
Алгоритм оценки описан ниже
## Детали расчета в разрезе реестров:

|                      Реестр                      |          Оценка          |  Оценка с учетом исключений  |                                    Ссылка на страницу валидаторов                                     |
|:------------------------------------------------:|:------------------------:|:----------------------------:|:-----------------------------------------------------------------------------------------------------:|
|                  **Стратегия**                   |      **{{strat}}**       |     **{{strat_except}}**     |          [Стратегия](/entities/kadzo.v2023.strategy/validation.errors_md?domain={{domain}})           |
|                     **Цели**                     |      **{{goals}}**       |     **{{goals_except}}**     |              [Цели](/entities/kadzo.v2023.goals/validation.errors_md?domain={{domain}})               |
|             **Клиенты**{{cl_errors}}             |     **{{clients}}**      |    **{{clients_except}}**    |            [Клиенты](/entities/kadzo.v2023.clients/validation.errors_md?domain={{domain}})            |
|                   **Продукты**                   |     **{{products}}**     |   **{{products_except}}**    |           [Продукты](/entities/kadzo.v2023.products/validation.errors_md?domain={{domain}})           |
|                    **Каналы**                    |     **{{channels}}**     |   **{{channels_except}}**    |            [Каналы](/entities/kadzo.v2023.channels/validation.errors_md?domain={{domain}})            |
|               **Бизнес-процессы**                |    **{{processes}}**     |   **{{processes_except}}**   |       [Бизнес-процессы](/entities/kadzo.v2023.processes/validation.errors_md?domain={{domain}})       |
|         **Бизнес-сущности**{{bo_errors}}         | **{{business_objects}}** |      **{{bo_except}}**       |   [Бизнес-сущности](/entities/kadzo.v2023.business_objects/validation.errors_md?domain={{domain}})    |
|                **Объекты данных**                |   **{{data_objects}}**   |      **{{do_except}}**       |      [Объекты данных](/entities/kadzo.v2023.data_objects/validation.errors_md?domain={{domain}})      |
|                **Задачи и планы**                |      **{{tasks}}**       |     **{{tasks_except}}**     |         [Задачи и планы](/entities/kadzo.v2023.tasks/validation.errors_md?domain={{domain}})          |
|               **Функциональность**               |    **{{functions}}**     |   **{{functions_except}}**   |      [Функциональность](/entities/kadzo.v2023.functions/validation.errors_md?domain={{domain}})       |
| **Автоматизированные системы**{{systems_errors}} |     **{{systems}}**      |    **{{systems_except}}**    |              [АС](/entities/kadzo.v2023.systems/validation.errors_md?domain={{domain}})               |
|                    **Группы**                    |      **{{groups}}**      |    **{{groups_except}}**     |             [Группы](/entities/kadzo.v2023.groups/validation.errors_md?domain={{domain}})             |
|            **Интеграционные потоки**             |   **{{integrations}}**   | **{{integrations_except}}**  |        [Интеграции](/entities/kadzo.v2023.integrations/validation.errors_md?domain={{domain}})        |
|                  **Системы КБ**                  |    **{{kb_systems}}**    |  **{{kb_systems_except}}**   |         [Системы КБ](/entities/kadzo.v2023.kb_systems/validation.errors_md?domain={{domain}})         |
|           **Технологические сервисы**            |  **{{tech_services}}**   | **{{tech_services_except}}** | [Технологические сервисы](/entities/kadzo.v2023.tech_services/validation.errors_md?domain={{domain}}) |
|                 **Параметры ТА**                 |   **{{tech_params}}**    |  **{{tech_params_except}}**  |       [Параметры ТА](/entities/kadzo.v2023.tech_params/validation.errors_md?domain={{domain}})        |
|                 **Точки взаимодействия**         |     **{{endpoints}}**    |   **{{endpoints_except}}**   |  [Точки взаимодействия](/entities/kadzo.v2023.endpoints/validation.errors_md?domain={{domain}})       |
|                **Кросс-проверки**                |      **{{cross}}**       |        **{{cross}}**         |    [Кросс проверки](/entities/kadzo.v2023.cross_validation/validation.errors_md?domain={{domain}})    |

## Дополнительные проверки
|                 Реестр                  |                          Ссылка на страницу валидаторов                          |
|:---------------------------------------:|:--------------------------------------------------------------------------------:|
|        **Домен**{{domain_error}}        | [Домен](/entities/kadzo.v2023.domain/validation.errors_md?domain={{domain}}) |
|  **Объединяющие элементы**{{MUEUsage}}  |  [Объединяющие элементы](/entities/kadzo.v2023.MUE/validation.errors_md?domain={{domain}})   |
| **Паспорта критичности**{{criticality}} |  [Паспорта критичности](/entities/kadzo.v2023.criticality_passport/validation.errors_md?domain={{domain}})   |

## Алгоритм оценки
По каждому из разделов и объектов, в них входящих, выполняются проверки, в случае возникновения ошибок оценка уменьшается.
В текущей версии функционала вес проверок равный между собой, а так же не учитываются заведенные исключения.

Оценка расчитывается по формуле:

Объект = ((ВесАтрибута1 * РезультатВалидации + ВесАтрибута2 * РезультатВалидации) * РезультатКритичнойВалидации) / СуммаВесов

РезультатВалидации принимает значение 1 при остутствии ошибок и 0 при их наличии.
РезультатКритичнойВалидации - это валидаторы по критичным атрибутам, позволяющим однозначино определить запись. К примеру наличие поля title.

Реестр = СуммаОбъектов / КоличествоОбъектов

ОбщаяОценка = СуммаРеестров / КоличествоРеестров
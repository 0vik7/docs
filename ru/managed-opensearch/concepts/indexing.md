# Индексы в {{ OS }}

Когда документ сохраняется в {{ OS }}, он индексируется и помещается в определенный _индекс_ по выбору пользователя, становясь доступным для поиска и анализа. Индекс можно рассматривать как аналог таблицы с данными в классических СУБД.

С точки зрения {{ OS }}, документ — это набор полей, где каждое поле — это пара `ключ: значение`. Индекс хранит документ в оптимизированном виде, чтобы обеспечить возможность быстрого поиска по полям в документе. Оптимизация достигается за счет того, что каждое поле документа имеет определенный тип — это позволяет эффективно хранить данные этого поля в индексе. Подробнее о такой оптимизации см. в [документации {{ OS }}]({{ os.docs }}/opensearch/mappings/).

В отличие от классических СУБД, {{ OS }} не требует явного задания схемы (взаимосвязей между полями документа и их типами), чтобы сохранить документ в индексе. Хотя это и рекомендуемый подход, можно сохранять документы в индекс без явного указания типа полей — {{ OS }} попытается определить тип автоматически для каждого поля документа. Это позволяет быстро наполнить хранилище {{ OS }} документами и начать работу с ними.

Подробнее об устройстве индексов см. в [документации {{ OS }}]({{ os.docs }}/opensearch/index-data/).

В многохостовых кластерах доступны [шардирование и репликация](scalability-and-resilience.md) индексов. Это упрощает масштабирование кластера и повышает его отказоустойчивость.
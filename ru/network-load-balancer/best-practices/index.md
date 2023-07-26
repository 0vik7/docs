# Общие рекомендации по использованию сетевого балансировщика

В статье представлен набор рекомендаций по использованию сетевого балансировщика {{ yandex-cloud }}.

#### Создавайте ресурсы в разных зонах доступности {#targets-in-different-azs}

Создавайте облачные ресурсы в нескольких зонах доступности. Так можно сохранить доступность ваших приложений при выходе из строя одной из зон.

#### Используйте одинаковое количество облачных ресурсов в разных зонах доступности {#equal-performance}

В каждой зоне доступности следует размещать одинаковое количество облачных ресурсов. Если в зоне доступности `{{ region-id }}-a` находятся три [виртуальных машины](../../glossary/vm.md), то и в зонах доступности `{{ region-id }}-b` и `{{ region-id }}-c` следует разместить по три виртуальных машины.

#### Создавайте облачные ресурсы с запасом {#redundancy}

Если одна из виртуальных машин в зоне доступности выйдет из строя, трафик продолжит поступать в зону доступности в том же объеме, увеличивая нагрузку на оставшиеся рабочие машины. Чтобы избежать выхода из строя всех машин, помимо ресурсов, необходимых для обслуживания расчетной нагрузки, рекомендуется использовать дополнительные ресурсы в каждой зоне доступности. 

#### Используйте отдельные балансировщики для разных приложений {#logical-distribution}

Если вы используете инфраструктуру {{ yandex-cloud }} для развертывания нескольких приложений, то следует настроить отдельные балансировщики для их обслуживания.

#### Организуйте многоуровневую инфраструктуру {#multi-layer-architecture}

Для увеличения надежности организуйте многоуровневую архитектуру с балансировщиками L3 и L7. L3-балансировщик будет принимать трафик и передавать его целевой группе L7-балансировщиков, которые будут распределять трафик по виртуальным машинам с приложениями. В качестве L7-балансировщиков можно использовать [{{ alb-name }}](../application-load-balancer/).

#### См. также {#see-also}

* [Особенности внутреннего балансировщика](internal-balancer-features.md)
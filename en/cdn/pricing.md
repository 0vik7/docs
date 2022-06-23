---
editable: false
---
# Pricing for {{ cdn-full-name }}

The cost of using {{ cdn-full-name }} is based on:

* The amount of outgoing traffic from CDN servers, including traffic requested by the user's {{ yandex-cloud }} resources, such as {{ compute-full-name}} [virtual machines](../compute/concepts/vm.md). The incoming traffic received by CDN servers from the {{ yandex-cloud }} services and resources or from the Internet, is not charged.

* Paid features enabled for resources, such as [origin shielding](concepts/origins-shielding.md) and [log export](concepts/logs.md).

  {% note info %}

  You will be billed for using paid functions starting October 1, 2021.

  {% endnote %}

## Pricing {#prices}

### Outgoing traffic {#traffic}




{% include notitle [usd.md](../_pricing/cdn/usd.md) %}


### Paid features {#paid-features}

Billing occurs on a monthly basis. If a function is enabled or disabled on any day of a month, the full monthly price will be charged for the month on the last day.




{% include notitle [usd-paid-features.md](../_pricing/cdn/usd-paid-features.md) %}



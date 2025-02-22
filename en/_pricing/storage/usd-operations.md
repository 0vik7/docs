| Service | Cost, without VAT |
| --- | --- |
| **Standard storage** |
| First 10,000 PUT operations per month | {{ sku|USD|storage.api.put.standard|string }} |
| First 10,000 POST operations per month | {{ sku|USD|storage.api.post.standard|string }} |
| First 10,000 PATCH operations per month | Free |
| First 100,000 GET operations per month | {{ sku|USD|storage.api.get.standard|string }} |
| First 100,000 HEAD operations per month | {{ sku|USD|storage.api.head.standard|string }} |
| First 100,000 OPTIONS operations per month | {{ sku|USD|storage.api.options.standard|string }} |
| 1,000 PUT operations | {{ sku|USD|storage.api.put.standard|pricingRate.10|string }} |
| 1,000 POST operations | {{ sku|USD|storage.api.post.standard|pricingRate.10|string }} |
| 1,000 PATCH operations | $0.003840 |
| 10,000 GET operations | {{ sku|USD|storage.api.get.standard|pricingRate.10|string }} |
| 10,000 HEAD operations | {{ sku|USD|storage.api.head.standard|pricingRate.10|string }} |
| 10,000 OPTIONS operations | {{ sku|USD|storage.api.options.standard|pricingRate.10|string }} |
| **Cold storage** |
| 1,000 PUT operations | {{ sku|USD|storage.api.put.cold|string }} |
| 1,000 POST operations | {{ sku|USD|storage.api.post.cold|string }} |
| 1,000 PATCH operations | $0.009440 |
| 10,000 GET operations | {{ sku|USD|storage.api.get.cold|string }} |
| 10,000 HEAD operations | {{ sku|USD|storage.api.head.cold|string }} |
| 10,000 OPTIONS operations | {{ sku|USD|storage.api.options.cold|string }} |
| **Ice storage** |
| 1,000 PUT operations | {{ sku|USD|storage.api.put.ice|string }} |
| 1,000 POST operations | {{ sku|USD|storage.api.post.ice|string }} |
| 1,000 PATCH operations | $0.018880 |
| 10,000 GET operations | {{ sku|USD|storage.api.get.ice|string }} |
| 10,000 HEAD operations | {{ sku|USD|storage.api.head.ice|string }} |
| 10,000 OPTIONS operations | {{ sku|USD|storage.api.options.ice|string }} |
# Domain to Stock Ticker mapping

A free to use dataset mapping the largest domains to Stock Ticker Symbols

## Dataset

### Top Domains
Top 10.000 domains (based on [Google Crux Ranking](https://developer.chrome.com/docs/crux) (deduplicated and removed subdomains) mapped to stock symbols.

### Top ecommerce Domains
Top 2.500 domains (based on [Gripsintelligence](https://gripsintelligence.com/)https://gripsintelligence.com/ (Dataset is focused on US and EU5 Countries)) mapped to stock symbols.

### Data Dictionary

|field|description|
| ------------- | ------------- |
|public_traded|yes or no if the domain belongs to a public traded company|
|ticker|	Exchange ticker, if the company is publicly traded|
|exchange|	Primary exchange where the company’s stock is traded, if public|
|market_cap|market capitalization|
|revenue|Revenue of the comapny based on last annual filling|
|no_employes|number of employees|
|founding_date|Year the company was founded|
|location|Headquarter location|
|related_domains|other domains related to the company|
|domain|initial checked domain|

## API (Alpha)

To get values for a given domain send a GET request specifiying the type, domain and your API-Key

Endpoint:

https://api.ticker-tagging.com/

|Name|Value/Type|Description|
| ------------- | ------------- | ------------- |
|type*|domain_tagging|The report type.|
|key*|API_KEY|An identification key assigned to the user after they subscribe.|
|domain*|amazon.com|The unique name of a website you'd like to investigate.|

Example:

https://api.ticker-tagging.com/?type=domain_tagging&key=YOUR_API_KEY&domain=amazon.com

## Contribution

If you want to contribute with a dataset (for example top x Traveldomains) we should tag and make public available reach out to: schmeh.daniel+tickertagging[at]gmail.com
Same if you want access to the early API Version.

# Netflix Prices Per Country

This repository contains data on Netflix subscription prices for different countries. The data is stored in JSON format and is updated regularly to reflect the latest prices.

## Data Structure

The **/data** folder contains JSON files named with the date (e.g., **2023-01-01.json**) as well as a file named **latest.json**, which contains the most recent prices.  
Each JSON file is a list of countries with the following structure:

```json
{
  "country_code": "AD",
  "country": "Andorra",
  "currency": "EUR",
  "plans": [
    {
      "name": "mobile",
      "price": null,
      "price_usd": null
    },
    {
      "name": "basic_with_ads",
      "price": null,
      "price_usd": null
    },
    {
      "name": "basic",
      "price": 7.99,
      "price_usd": 8.7
    },
    {
      "name": "standard_with_ads",
      "price": null,
      "price_usd": null
    },
    {
      "name": "standard",
      "price": 12.99,
      "price_usd": 14.15
    },
    {
      "name": "premium",
      "price": 17.99,
      "price_usd": 19.6
    }
  ]
}
```

*   **country_code**: The 2-letter ISO country code (e.g., "AD" for Andorra).
*   **country**: The full country name.
*   **currency**: The 3-letter ISO currency code (e.g., "EUR" for Euro).
*   **plans**: A list of dictionaries, each containing the following keys:
    *   **name**: The Netflix subscription plan (e.g., "mobile", "basic_with_ads", "basic", "standard_with_ads", "standard", "premium").
    *   **price**: The price of the subscription plan in the local currency. If the price is `null`, it means that the plan is not available in this country.
    *   **price_usd**: The price of the subscription plan in USD.

## Usage

You can use this data to analyze Netflix subscription prices across different countries and currencies. Some possible use cases include:

*   Comparing prices between countries.
*   Identifying trends in subscription prices over time.
*   Evaluating the impact of currency exchange rates on subscription prices.

Feel free to use the data in your own projects or research. Please give proper credit if you use this data in any publicly available material.

## Attribution

If you use this work in any publicly available material, please attribute the original creation by including a link to [thomas.io](https://www.thomas.io).

## License

This work is licensed under the [Creative Commons Attribution 4.0 International License](/LICENSE.md). To view a copy of this license, visit http://creativecommons.org/licenses/by/4.0/ or see the [LICENSE](/LICENSE.md) file.

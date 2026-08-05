# predictorsdk

The official Python client for the [PredictorSDK](https://predictorsdk.com) prediction-market data API.

## Installation

```bash
pip install predictorsdk
```

## Usage

```python
from predictorsdk import PredictorSDK

client = PredictorSDK(token="your-api-key")

plans = client.get_plans()
categories = client.get_categories()
markets = client.get_markets(limit=10, category="sports")

print(plans.data, categories.data, markets.data)
```

## Documentation

- [Docs](https://docs.predictorsdk.com)
- [API Reference](https://docs.predictorsdk.com/api-reference)

## License

[MIT](https://github.com/PredictorSDK/sdk-python/blob/main/LICENSE)

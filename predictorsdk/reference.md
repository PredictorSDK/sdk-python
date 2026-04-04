# Reference
<details><summary><code>client.<a href="src/predictorsdk/client.py">get_sports_matching_markets</a>(...) -> SportsMatchingResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Find cross-platform market matches for sports events. Provide a Kalshi event ticker or Polymarket market slug to look up the equivalent market on other platforms. When called without parameters, returns all currently matched sports markets.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```python
from predictorsdk import PredictorSdkApi
from predictorsdk.environment import PredictorSdkApiEnvironment

client = PredictorSdkApi(
    token="<token>",
    environment=PredictorSdkApiEnvironment.PRODUCTION,
)

client.get_sports_matching_markets()

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**kalshi_event_ticker:** `typing.Optional[typing.Union[str, typing.Sequence[str]]]` — Kalshi event ticker(s) to find matching markets for (e.g. `KXNFLGAME-25AUG16ARIDEN`). Provide the parameter multiple times for multiple tickers. Only one filter type may be used per request.
    
</dd>
</dl>

<dl>
<dd>

**polymarket_market_slug:** `typing.Optional[typing.Union[str, typing.Sequence[str]]]` — Polymarket market slug(s) to find matching markets for (e.g. `nfl-ari-den-2025-08-16`). Provide the parameter multiple times for multiple slugs. Only one filter type may be used per request.
    
</dd>
</dl>

<dl>
<dd>

**predict_market_id:** `typing.Optional[typing.Union[str, typing.Sequence[str]]]` — Predict market ID(s) to find matching markets for (e.g. `110629`). Provide the parameter multiple times for multiple IDs. Only one filter type may be used per request.
    
</dd>
</dl>

<dl>
<dd>

**sxbet_market_id:** `typing.Optional[typing.Union[str, typing.Sequence[str]]]` — SX Bet market ID(s) to find matching markets for (e.g. `0x4c000abdbf197ef32ecdf15561b1d636f1e5b02629f466678757fd83e2ec3599`). Provide the parameter multiple times for multiple IDs. Only one filter type may be used per request.
    
</dd>
</dl>

<dl>
<dd>

**request_options:** `typing.Optional[RequestOptions]` — Request-specific configuration.
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>


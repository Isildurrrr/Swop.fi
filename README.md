# Swop.fi
Json for swop.fi
## Pools
1) USDN/USDT: 3PPH7x7iqobW5ziyiRCic19rQqKr6nPYaK1
2) USDN/NSBT: 3P2V63Xd6BviDkeMzxhUw2SJyojByRz8a8m
3) WAVES/USDN: 3PHaNgomBkrvEL2QnuJarQVJa71wjw9qiqG
4) sUSDLP_USD-N: 3PDWi8hjQJjXhyTpeaiEYfFKWBd1iC4udfF

## Token ID's
1) sNSBT_USD-N:  HWFcdC9wjPJY1udkR2UsfXzyPptzBb9m6df8qUW6LNLo
2) sUSDT_USD-N:  BNQ8bxyiWvfHzHAtNyfc6E7v3sSHXKq8yuit6Fnz1A3Q
3) WAVES/USDN: Btw3G1j4wQgdp49PTxaFkNvn75dQtqGDM7ejQppHnWC1
4) sUSDLP_USD-N: 9Pm2c97VzGSK6p8XGMCFABs575K9Cb35GdKtzwVA59m9

## Stake usdn/usdt token to farming pool

String value = dapp from pool

AssetId = assetId from pool token
```

{
  "type": 16,
  "version": 2,
  "dApp": "3P73HDkPqG15nLXevjCbmXtazHYTZbpPoPw",
  "call": {
    "args": [
      {
        "type": "string",
        "value": "3PPH7x7iqobW5ziyiRCic19rQqKr6nPYaK1"
      }
    ],
    "function": "lockShareTokens"
  },
  "payment": [
    {
      "assetId": "BNQ8bxyiWvfHzHAtNyfc6E7v3sSHXKq8yuit6Fnz1A3Q",
      "amount": "1000000"
    }
  ],
  "fee": 500000,
  "feeAssetId": null,
  "chainId": 87
}
```

## Unstake NSBT/USDN
String value = dapp from pool

```

{
    "type": 16,
    "version": 2,
    "dApp": "3P73HDkPqG15nLXevjCbmXtazHYTZbpPoPw",
    "call": {
        "args": [
            {
                "type": "string",
                "value": "3P2V63Xd6BviDkeMzxhUw2SJyojByRz8a8m"
            },
            {
                "type": "integer",
                "value": 1000000
            }
        ],
        "function": "withdrawShareTokens"
    },
    "payment": [],
    "fee": 500000,
    "feeAssetId": null,
    "chainId": 87
}
```

## Claim swop early bird

```
{
  "type": 16,
  "fee": 500000,
  "feeAssetId": null,
  "version": 2,
  "chainId": 87,
  "dApp": "3PJuspTjxHhEJQjMEmLM5upiGQYCtCi5LyD",
  "payment": [],
  "call": {
    "function": "claimSWOP",
    "args": []
  }
  }
  ```

## Claim normal swop
String Value = pool dapp address
  ```
{
  "type": 16,
  "version": 2,
  "dApp": "3P73HDkPqG15nLXevjCbmXtazHYTZbpPoPw",
  "call": {
    "args": [
      {
        "type": "string",
        "value": "3PPH7x7iqobW5ziyiRCic19rQqKr6nPYaK1"
      }
    ],
    "function": "claim"
  },
  "payment": [],
  "fee": 500000,
  "feeAssetId": null,
  "chainId": 87,
  "proofs": []
}
  ```
## Governance token stake /Lock swop
  ```
{
  "type": 16,
  "version": 2,
  "dApp": "3PLHVWCqA9DJPDbadUofTohnCULLauiDWhS",
  "call": {
    "args": [ ],
    "function": "lockSWOP"
  },
  "payment": [
    {
      "assetId": "Ehie5xYpeN8op1Cctc6aGUrqx8jq3jtf1DSjXDbfm7aT",
      "amount": "100000000"
    }
  ],
  "fee": 500000,
  "feeAssetId": null,
  "chainId": 87
}
  ```
  
## Governance token wd
  ```
{
  "type": 16,
  "version": 2,
  "dApp": "3PLHVWCqA9DJPDbadUofTohnCULLauiDWhS",
  "call": {
    "args": [
      {
        "type": "integer",
        "value": 100000000
      }
    ],
    "function": "withdrawSWOP"
  },
  "payment": [],
  "fee": 500000,
  "feeAssetId": null,
  "chainId": 87
}
  ```

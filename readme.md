# Technical test

## Context

In this test, you have to implement a simple second price sealed-bid auction.

- There are several buyers who can place one or more bids on one or more categories
- The auction winner is the one with the highest bid over the floor price for the given category
- The effective price is the price of the second best bids (without self-competing) and above the floor price

## Example

Consider 5 buyers (A, B, C, D, E) for the auction 0.7 in category I

- A Category I prices  0.3, 0.75, 0.89
- B Category II prices 0.99
- C Category I prices 0.73
- D Category III prices  0.39, 0.85, 0.88
- E Category I prices 0.5

The Winner will be A with an effective price of 0.73

### Objectives

1. implement an algorithm to find the auction winner without category
2. implement an algorithm to find the auction winner with category
3. implement an algorithm to find the effective price
4. implement an interactive version that receives an auction and provides the result as described

### Guidelines

- Use Python
- Push your code to a Github repository
- Document what you've done

### Evaluation

- Answer as many points as possible
- Quality of the code
- Usage of good practices
- Quality of the algorithm

## Data format

### Buyers

```json
 {
            "name": "aive",
            "bids": [
                {
                    "category": "IAB6",
                    "prices": [
                        0.17,
                        0.46,
                        0.87
                    ]
                },
                {
                    "category": "IAB1",
                    "prices": [
                        0.37
                    ]
                }
            ]
        }
```

### Auctions

```json
{
    "domain": "geotrust.com",
    "price": 0.79,
    "category": "IAB2"
}
```

### Output format

```json
{
"results": [
        {
            "effective_price": 0.0,
            "advertiser": {
                 "name": "",
                 "catgeory":""
            }
        }
    ]
}
```

***There is no time limit, have fun!***

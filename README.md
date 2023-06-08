# ida

## Abstract

Ideas might be the most valuable information we could think to put on-chain: they have the lowest risk profile of any asset and can be represented in digital form very cheaply. The cost of an idea can be zero and the potential return infinity. Ideas can also be easily capitalized on.

Bitcoin is a hive mind and proof-of-work is the mechanism for filtering the good ideas from the bad with byzantine fault tolerance. 

`ida` is a protocol for publishing new ideas on-chain and an indexer for these ideas. It relies on [Boost POW](https://media.bitcoinfiles.org/52fb4bedc85854638af61a7f906bf8e93da847d2ddb522b1aec53cfc6a0b2023) protocol to filter these ideas.

You can think of `ida` as an abstract flag - many more flags, with many more levels of detail, will be used by other Boost applications. `ida` is simply the first metadata tag dedicated to flagging content as a new idea. 

## Usage

Add the following metadata to any object to request it to be indexed:
```
    ida: 1
```

Example: [Ordinal News Standard](https://docs.inscribe.news/) inscription using `ida` protocol:
```
{
  "p": "ons",
  "op": "post",
  "title": "make the bitcoin whitepaper required reading in high schools",
  "ida": 1,
}
```

You will notice `ida` is intentionally not used in the `p` protocol field. It is simply metadata. Where on the object it lives is arbitrary.

## What's next

You tell me.

## Disclaimer

> ⚠️ this is a work in progress protocol with no API or interfaces built

> 🛑 use at your own risk
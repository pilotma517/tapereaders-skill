# Tape Readers — agent skill

An agent skill for **Tape Readers**, a collection of 2,000 fully on-chain trading-robot NFTs on BNB Chain that only
AI agents can mint (the minting wallet must hold a SPACE ID Agent ID, i.e. a Binance Agentic Wallet with a `.ai` name).

The skill teaches an agent to:

- check whether the user's wallet can mint, and how many it can still mint
- mint after the user explicitly confirms (contract call, or a plain BNB transfer)
- read the on-chain order book and buy, list, bid or sell on the collection's market, again only after confirmation

It never holds keys: transactions go through the user's own wallet tooling (for Binance Agentic Wallet, `baw
contract-call preview` → user confirms → `execute`).

## Use it

Give your agent the skill file:

```
https://raw.githubusercontent.com/pilotma517/tapereaders-skill/main/tape-readers/SKILL.md
```

or say: *"Read the Tape Readers skill at the link above and check whether my wallet can mint."*

## Links

- Website: https://tapereaders.netlify.app
- NFT contract (BNB Chain): [`0x0f05a8e1f6b04BB5d657e20305F86ff411B998C2`](https://bscscan.com/address/0x0f05a8e1f6b04BB5d657e20305F86ff411B998C2#code), source verified on BscScan and Sourcify
- Market contract (BNB Chain): [`0xEAd55ED2cDb6855E9CfB709199Bba951cEa39169`](https://bscscan.com/address/0xEAd55ED2cDb6855E9CfB709199Bba951cEa39169#code), source verified

## Notes

- Digital collectibles. Nothing here is investment advice, and no returns are promised.
- Independent project, not affiliated with Binance or SPACE ID; the Agent ID is only used as the mint gate.
- Always verify contract addresses against this README and BscScan before sending a transaction.

## License

MIT

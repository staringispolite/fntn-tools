# fntn-tools
Solidity utility contract for ✨doing things✨ with FNTN shards

```
> git clone [...]
> cd fntn-tools
> yarn
> truffle compile
> truffle test
```

```solidity
contract myContract is FNTNConverter {

  function foo(uint shardNumber) public {
    uint originalTokenId = shardIdToTokenId(shardNumber);
  }

}
```

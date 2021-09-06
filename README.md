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
    // Get tokenId in original FNTN contract
    uint originalTokenId = shardIdToTokenId(shardNumber);
    
    // Ensure the sender owns this shard
    require(fntnContract.ownerOf(originalTokenId) == msg.sender);
  }

}
```

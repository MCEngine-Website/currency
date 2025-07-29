## `getCoin(UUID uuid, String coinType)`

> **Description:**  
Retrieves the current coin balance for a player.

### Function
```java
public double getCoin(UUID uuid, String coinType)
```

### Usage
```java
double coins = common.getCoin(playerId, "copper");
```

### Summary
Returns the balance of the requested coin type for a player.

## `createTransaction(...)`

> **Description:**  
Records a economy transaction between two players.

### Function
```java
public void createTransaction(
  UUID sender,
  UUID receiver,
  String currencyType,
  String transactionType,
  double amount,
  String notes
)
```

### Usage
```java
common.createTransaction(senderId, receiverId, "gold", "pay", 10.0, "Payment for item");
```

### Summary
Logs a transaction with type, economy, amount, and optional notes.

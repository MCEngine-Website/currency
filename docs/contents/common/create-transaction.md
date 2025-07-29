## `createTransaction(...)`

> **Description:**  
Records a currency transaction between two players.

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
Logs a transaction with type, currency, amount, and optional notes.

# Currency API Module Usage Guide

**Path:** `com.example.MyCurrencyAPI.java`
[`Example Repository`](https://github.com/MCEngine-Extension/economy-api-example)

This document explains how to implement the `IMCEngineCurrencyAPI` interface to create a central currency API module for the MCEngine.

## Interface

```java
package com.example;

import io.github.mcengine.api.currency.extension.api.IMCEngineCurrencyAPI;
import io.github.mcengine.api.core.extension.logger.MCEngineExtensionLogger;
import org.bukkit.plugin.Plugin;

public class MyCurrencyAPI implements IMCEngineCurrencyAPI {

    private String id;

    @Override
    public void onLoad(Plugin plugin) {
        MCEngineExtensionLogger logger = new MCEngineExtensionLogger(plugin, "API", id);
        logger.info("Currency API loaded with ID: " + id);
    }

    @Override
    public void onDisload(Plugin plugin) {
        MCEngineExtensionLogger logger = new MCEngineExtensionLogger(plugin, "API", id);
        logger.info("Currency API unloaded with ID: " + id);
    }

    @Override
    public void setId(String id) {
        MCEngineApi.setId("example");
    }
}
```

## Description

This interface serves as the core API layer for currency systems. It should manage balances, currency types, and cross-module integrations.

## Notes

- Ideal for backend processing and economy logic.
- Avoid direct player events in the API; delegate to AddOns or DLCs.

# Currency DLC Module Usage Guide

**Path:** `com.example.MyCurrencyDLC.java`
[`Example Repository`](https://github.com/MCEngine-Extension/economy-dlc-example)

This document explains how to implement the `IMCEngineCurrencyDLC` interface to create a currency-based DLC for the MCEngine.

## Interface

```java
package com.example;

import io.github.mcengine.api.currency.extension.dlc.IMCEngineCurrencyDLC;
import io.github.mcengine.api.core.extension.logger.MCEngineExtensionLogger;
import org.bukkit.plugin.Plugin;

public class MyCurrencyDLC implements IMCEngineCurrencyDLC {

    private String id;

    @Override
    public void onLoad(Plugin plugin) {
        MCEngineExtensionLogger logger = new MCEngineExtensionLogger(plugin, "DLC", id);
        logger.info("Currency DLC loaded with ID: " + id);
    }

    @Override
    public void onDisload(Plugin plugin) {
        MCEngineExtensionLogger logger = new MCEngineExtensionLogger(plugin, "DLC", id);
        logger.info("Currency DLC unloaded with ID: " + id);
    }

    @Override
    public void setId(String id) {
        MCEngineApi.setId("example");
    }
}
```

## Description

This interface enables modular content packs that leverage or enhance currency systems—like shop systems, trade expansions, or currency quests.

## Notes

- Use `onLoad` to add new economy-related content.
- Ensure proper cleanup in `onDisload` to prevent dangling hooks.

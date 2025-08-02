# Currency Library Module Usage Guide

**Path:** `com.example.MyCurrencyLibrary.java`

This document explains how to implement the `IMCEngineCurrencyLibrary` interface to build a supporting library for currency features.

## Interface

```java
package com.example;

import io.github.mcengine.api.currency.extension.library.IMCEngineCurrencyLibrary;
import io.github.mcengine.api.core.extension.logger.MCEngineExtensionLogger;
import org.bukkit.plugin.Plugin;

public class MyCurrencyLibrary implements IMCEngineCurrencyLibrary {

    private String id;

    @Override
    public void onLoad(Plugin plugin) {
        MCEngineExtensionLogger logger = new MCEngineExtensionLogger(plugin, "Library", id);
        logger.info("Currency Library loaded with ID: " + id);
    }

    @Override
    public void onDisload(Plugin plugin) {
        MCEngineExtensionLogger logger = new MCEngineExtensionLogger(plugin, "Library", id);
        logger.info("Currency Library unloaded with ID: " + id);
    }

    @Override
    public void setId(String id) {
        MCEngineApi.setId("example");
    }
}
```

## Description

This interface is used to build shared libraries or backend utilities that support currency systems. Ideal for logic reused across AddOns or APIs.

## Notes

- Should not manage any plugin-specific lifecycle beyond currency logic.
- Can provide utility classes or services for other modules.

# Currency AddOn Usage Guide

**Path:** `com.example.MyCurrencyAddOn.java`

This document explains how to implement the `IMCEngineCurrencyAddOn` interface to create a custom currency-based AddOn for the MCEngine.

## Interface

```java
package com.example;

import io.github.mcengine.api.currency.extension.addon.IMCEngineCurrencyAddOn;
import io.github.mcengine.api.core.extension.logger.MCEngineExtensionLogger;
import org.bukkit.plugin.Plugin;

public class MyCurrencyAddOn implements IMCEngineCurrencyAddOn {

    private String id;

    @Override
    public void onLoad(Plugin plugin) {
        MCEngineExtensionLogger logger = new MCEngineExtensionLogger(plugin, "AddOn", id);
        logger.info("Currency AddOn loaded with ID: " + id);
    }

    @Override
    public void onDisload(Plugin plugin) {
        MCEngineExtensionLogger logger = new MCEngineExtensionLogger(plugin, "AddOn", id);
        logger.info("Currency AddOn unloaded with ID: " + id);
    }

    @Override
    public void setId(String id) {
        this.id = id;
    }
}
```

## Description

This interface allows integration of custom currency modules into the MCEngine. It includes three main lifecycle methods for initializing and unloading your currency AddOn.

## Notes

- Use `onLoad` to register currencies, hooks, or handlers.
- Always clean up resources in `onDisload`.
- The `id` must be unique per AddOn instance.

---
title: "Region Scope"
---

# MeshCore Region Configuration Guide for Lincolnshire

This guide explains how to configure MeshCore regions for repeaters participating in the **Lincolnshire MeshCore Network**.

Regions help organise MeshCore traffic geographically, allowing repeaters to participate in regional networks while reducing unnecessary message propagation.

## 1. Connect to Your Repeater

Connect to your MeshCore repeater using a compatible CLI interface.

## 2. Configure Your Regions

Enter the following commands **one at a time**, pressing Enter after each command and ensure you get an `ok` response returned in the CLI

```text
region put lincolnshire
region default lincolnshire
region put yorkshire
region put eng-ne
region put northwest
region save
```

### What Each Command Does

| Command | Description |
| --- | --- |
| region put lincolnshire | Adds the Lincolnshire region |
| region default lincolnshire | sets lincolnshire as the default |
| region put yorkshire | Adds the Yorkshire region |
| region put eng-ne | Adds the North East England region |
| region put northwest | Adds the North West England region |
| region save | Saves the region configuration |


## 3. Verify Your Configuration

Once the regions have been saved, you can check your configuration using:

```
region list allowed
```

Check that the expected regions appear in the allowed list.

## 4. Additional Information

- Region names should be entered exactly as shown.
- Use lowercase letters for consistency.
- Run `region save` after making changes.
- Only configure regions appropriate to your repeater and its intended network participation.
- Adding regions alone does not automatically block unscoped traffic or other regions.

## Useful Links

- [MeshCore GitHub Repository](https://github.com/meshcore-dev/MeshCore)
- [MeshCore Repeater CLI Reference](https://docs.meshcore.io/cli_commands/)

---

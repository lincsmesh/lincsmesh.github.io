---
title: "Home"
---
![Meshcore Logo](/assets/meshcore-tm.avif)

Welcome to the landing page of the Lincolnshire [Meshcore](https://meshcore.io).

# What is Meshcore?

# Getting Started
test

# Settings  

# MeshCore Region Configuration Guide

This guide explains how to configure MeshCore regions for repeaters participating in the **Lincolnshire MeshCore Network**.

Regions help organise MeshCore traffic geographically, allowing repeaters to participate in regional networks while reducing unnecessary message propagation.

## 1. Connect to Your Repeater

Connect to your MeshCore repeater using a compatible CLI interface.

## 2. Configure Your Regions

Enter the following commands **one at a time**, pressing Enter after each command.

```text
region put lincolnshire
region put yorkshire
region put eng-ne
region put northwest
region save
```

### What Each Command Does

| Command | Description |
|---------|-------------|
| `region put lincolnshire` | Adds the Lincolnshire region |
| `region put yorkshire` | Adds the Yorkshire region |
| `region put eng-ne` | Adds the North East England region |
| `region put northwest` | Adds the North West England region |
| `region save` | Saves the region configuration |

## 3. Important – Default Region

**⚠️ Do not configure a default region yet.**

The following command is **NOT currently required**:

```text
region default lincolnshire
```

This setting may be introduced at a later stage as the regional network configuration develops.

For now, only use the commands provided in Section 2.

## 4. Verify Your Configuration

Once the regions have been saved, you can check your configuration using:

```text
region list allowed
```

Check that the expected regions appear in the allowed list.

## 5. Additional Information

- Region names should be entered exactly as shown.
- Use lowercase letters for consistency.
- Run `region save` after making changes.
- Only configure regions appropriate to your repeater and its intended network participation.
- Adding regions alone does not automatically block unscoped traffic or other regions.

## Useful Links

- [MeshCore GitHub Repository](https://github.com/meshcore-dev/MeshCore)
- [MeshCore Repeater CLI Reference](https://github.com/meshcore-dev/MeshCore/wiki/Repeater-%26-Room-Server-CLI-Reference)

---

**Lincolnshire MeshCore Community**

Helping build a reliable and connected MeshCore network across Lincolnshire and neighbouring regions.


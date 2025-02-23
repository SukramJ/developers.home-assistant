---
title: "The documentation describes the supported functionality, including entities, and platforms"
---

## Reasoning

Users should be able to understand what value the integration will add for their (to be bought) device.
This will help set users' expectations.

For example, if a user is looking for a new fridge, we should try to be clear about what they can expect from the integration.
If the integration only supports checking if the door is open or closed, they would be disappointed if they expected to be able to view the temperature of the fridge.

## Example implementation

Example, sorted by entity types:

```markdown showLineNumbers
## Supported functionality

### Entities

The XY integration provides the following entities.

#### Buttons

- **Start backflush**
  - **Description**: Starts the backflush process on your machine. You got 15 seconds to turn the paddle after activation.
  - **Available for machines**: all

#### Numbers

- **Dose**
  - **Description**: Dosage (in ticks) for each key
  - **Available for machines**: GS3 AV, Linea Mini.
  - **Remarks**: GS3 has this multiple times, one for each physical key (1-4), and the entities are disabled by default.

#### Sensors

- **Current coffee temperature**
  - **Description**: Current temperature of the coffee boiler.
  - **Available for machines**: all
  - **Remarks**: When the machine reaches temperature, this will be approximately 3 degrees higher than the `Coffee target temperature`, due to different measurement points.

- **Current steam temperature**
  - **Description**: Current temperature of the steam boiler.
  - **Available for machines**: Linea Micra, GS3 AV, GS3 MP.
  - **Remarks**: -

#### Updates

- **Gateway firmware**
  - **Description**: Firmware status of the gateway.
  - **Available for machines**: all

#### Selects

- **Prebrew/-infusion mode**
  - **Description**: Whether to use prebrew, preinfusion, or neither.
  - **Options**: Disabled, Prebrew, Preinfusion
  - **Available for machines**: Linea Micra, Linea Mini, GS3 AV

- **Steam level**
  - **Description**: The level your steam boiler should run at.
  - **Options**: 1, 2, 3
  - **Available for machines**: Linea Micra
```

Example, sorted by device:

```markdown
## Supported functionality

### XYZ productname Air Purifier, Air Humidifier and Standing Fan

#### Sensors

- **Filter lifetime remaining**: The remaining life of the filter in number of years. Enabled by default.
- **Purify volume**: The volume of purified air in cubic meters. Disabled by default.

#### Numbers

- **Favorite level**: Set the favorite level. Possible values are 0 to 10. `0` means it is turned off.)
- **Volume**: Set the volume. In percent. `0%` means it is off.
```

## Exceptions

There are no exceptions to this rule.
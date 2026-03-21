# Soft Biometric Attribute Documentation

This document describes all attribute labels used in the DetReIDX dataset, including encoding values, file naming conventions, and example filenames.

---

## Attribute Reference Tables

### Biometric Attributes

#### Gender
| Label | Description |
|-------|-------------|
| `0`   | Male        |
| `1`   | Female      |
| `2`   | Other       |

#### Age
| Label | Description |
|-------|-------------|
| `0`   | 0–11        |
| `1`   | 12–17       |
| `2`   | 18–24       |
| `3`   | 25–34       |
| `4`   | 35–44       |
| `5`   | 45–54       |
| `6`   | 55–67       |
| `7`   | 65+         |
| `-1`  | Unknown     |

#### Height
| Label | Description          |
|-------|----------------------|
| `0`   | Child — below 150 cm |
| `1`   | Short — 150–160 cm   |
| `2`   | Medium — 160–170 cm  |
| `3`   | Tall — above 170 cm  |
| `-1`  | Unknown              |

#### Weight
| Label | Description          |
|-------|----------------------|
| `0`   | Thin — below 60 kg   |
| `1`   | Medium — 60–80 kg    |
| `2`   | Heavy — above 80 kg  |
| `-1`  | Unknown              |

#### Ethnicity
| Label | Description    |
|-------|----------------|
| `0`   | Indian         |
| `1`   | Black          |
| `2`   | Turkish/White  |
| `3`   | White          |

---

### Appearance Attributes

#### Hair Color
| Label | Description |
|-------|-------------|
| `0`   | Black       |
| `1`   | Brown       |
| `2`   | White       |
| `3`   | Red         |
| `4`   | Gray        |
| `5`   | Occluded    |
| `-1`  | Unknown     |

#### Hair Style
| Label | Description |
|-------|-------------|
| `0`   | Bald        |
| `1`   | Short       |
| `2`   | Medium      |
| `3`   | Long        |
| `4`   | Ponytail    |
| `-1`  | Unknown     |

#### Beard
| Label | Description |
|-------|-------------|
| `0`   | Yes         |
| `1`   | No          |
| `-1`  | Unknown     |

#### Moustache
| Label | Description |
|-------|-------------|
| `0`   | Yes         |
| `1`   | No          |
| `-1`  | Unknown     |

#### Glasses
| Label | Description  |
|-------|--------------|
| `0`   | Regular      |
| `1`   | Sunglasses   |
| `-1`  | Unknown      |

#### Head Accessories
| Label | Description  |
|-------|--------------|
| `0`   | Hat          |
| `1`   | Scarf        |
| `2`   | Necklace     |
| `3`   | Not visible  |
| `-1`  | Unknown      |

---

### Clothing Attributes

#### Upper Body
| Label | Description |
|-------|-------------|
| `0`   | T-Shirt     |
| `1`   | Blouse      |
| `2`   | Sweater     |
| `3`   | Coat        |
| `4`   | Dress       |
| `5`   | Uniform     |
| `6`   | Shirt       |
| `7`   | Suit        |
| `8`   | Hoodie      |
| `-1`  | Unknown     |

#### Lower Body
| Label | Description |
|-------|-------------|
| `0`   | Jeans       |
| `1`   | Leggings    |
| `2`   | Pants       |
| `3`   | Shorts      |
| `4`   | Skirt       |
| `5`   | Dress       |
| `6`   | Uniform     |
| `7`   | Suit        |
| `-1`  | Unknown     |

#### Footwear
| Label | Description   |
|-------|---------------|
| `0`   | Sports Shoes  |
| `1`   | Classic Shoes |
| `2`   | High Heels    |
| `3`   | Boots         |
| `4`   | Sandals       |
| `5`   | Barefoot      |
| `-1`  | Unknown       |

#### Accessories
| Label | Description   |
|-------|---------------|
| `0`   | Handbag       |
| `1`   | Backpack      |
| `2`   | Rolling Bag   |
| `3`   | Umbrella      |
| `4`   | Sports Bag    |
| `5`   | Market Bag    |
| `6`   | None          |
| `-1`  | Unknown       |

---

## File Naming Conventions

### Indoor Images & Gait Videos

Format:
```
PID_Gender_Age_Height_Weight_Ethnicity_Angle_View.ext
```

| Field      | Description                            |
|------------|----------------------------------------|
| `PID`      | 4-digit zero-padded person ID          |
| `Gender`   | Encoded gender label (see above)       |
| `Age`      | Encoded age group label                |
| `Height`   | Encoded height category                |
| `Weight`   | Encoded weight category                |
| `Ethnicity`| Encoded ethnicity label                |
| `Angle`    | Camera angle in degrees                |
| `View`     | `F` = Front, `L` = Left, `R` = Right  |

**Example:**
```
0001_0_2_2_1_0_45_F.jpg
```
→ Person 0001 | Male | Age 18–24 | Height 160–170 cm | Weight 60–80 kg | Indian | 45° | Front view

---

### Outdoor Images (UAV / Drone)

Format:
```
PID_Date_Time_DroneHeight_Distance_Angle_Location_HairColor_HairStyle_Beard_Moustache_Glasses_HeadAccessories_UpperBody_LowerBody_Feet_Accessories_Action_DroneScene_SessionID.ext
```

| Field             | Description                                    |
|-------------------|------------------------------------------------|
| `PID`             | 4-digit zero-padded person ID                  |
| `Date`            | Capture date as `DD_MM_YYYY`                   |
| `Time`            | Capture time as `HH_MM`                        |
| `DroneHeight`     | Drone altitude in meters                       |
| `Distance`        | Distance from subject in meters               |
| `Angle`           | Camera pitch angle in degrees                  |
| `Location`        | Location ID                                    |
| `HairColor`       | Encoded hair color                             |
| `HairStyle`       | Encoded hair style                             |
| `Beard`           | Beard presence                                 |
| `Moustache`       | Moustache presence                             |
| `Glasses`         | Glasses type                                   |
| `HeadAccessories` | Head accessory label                           |
| `UpperBody`       | Upper clothing label                           |
| `LowerBody`       | Lower clothing label                           |
| `Feet`            | Footwear label                                 |
| `Accessories`     | Carried accessory label                        |
| `Action`          | Encoded action/behavior                        |
| `DroneScene`      | Drone scene number                             |
| `SessionID`       | Session identifier (e.g., `S1`, `S2`)         |

**Example:**
```
0004_23_10_2024_09_18_5.8_10_30_3_0_1_1_0_-1_-1_6_0_0_6_152_178_S1.jpg
```
→ Person 0004 | Oct 23 2024 | 09:18 | 5.8m height | 10m distance | 30° angle | Location 3 | ...

---

## License

This dataset is released for **academic and non-commercial use only**.
See the [main README](README.md) for full license and citation information.

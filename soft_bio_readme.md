# Dataset README

This README provides detailed information about the dataset attributes and the corresponding labels. 

## Dataset Description

This dataset contains annotated information for attributes related to gender, age, height, weight, ethnicity, and various other features. These attributes are encoded with specific values to enable efficient analysis and machine learning applications.

---

## Attribute Details

### Gender
| Label   | Description |
|---------|-------------|
| 0       | Male        |
| 1       | Female      |
| 2       | Other       |

### Age
| Label   | Description |
|---------|-------------|
| 0       | 0-11        |
| 1       | 12-17       |
| 2       | 18-24       |
| 3       | 25-34       |
| 4       | 35-44       |
| 5       | 45-54       |
| 6       | 55-67       |
| 7       | >65         |
| -1      | Unknown     |

### Height
| Label   | Description           |
|---------|-----------------------|
| 0       | Child: Below 150 cm  |
| 1       | Short: 150 - 160 cm  |
| 2       | Medium: 160 - 170 cm |
| 3       | Tall: Above 170 cm   |
| -1      | Unknown              |

### Weight
| Label   | Description            |
|---------|------------------------|
| 0       | Thin: Below 60 kg    |
| 1       | Medium: 60 - 80 kg   |
| 2       | Fat: Above 80 kg     |
| -1      | Unknown              |

### Ethnicity
| Label   | Description |
|---------|-------------|
| 0       | Indian      |
| 1       | Black       |
| 2       | Turkish White |
| 3       | White       |

### Hair Color
| Label   | Description |
|---------|-------------|
| 0       | Black       |
| 1       | Brown       |
| 2       | White       |
| 3       | Red         |
| 4       | Gray        |
| 5       | Occluded    |
| -1      | Unknown     |

### Hair Style
| Label   | Description |
|---------|-------------|
| 0       | Bald        |
| 1       | Short       |
| 2       | Medium      |
| 3       | Long        |
| 4       | Horse Tail  |
| -1      | Unknown     |

### Beard
| Label   | Description |
|---------|-------------|
| 0       | Yes         |
| 1       | No          |
| -1      | Unknown     |

### Moustache
| Label   | Description |
|---------|-------------|
| 0       | Yes         |
| 1       | No          |
| -1      | Unknown     |

### Glasses
| Label   | Description |
|---------|-------------|
| 0       | Normal      |
| 1       | Sun         |
| -1      | Unknown     |

### Head Accessories
| Label   | Description |
|---------|-------------|
| 0       | Hat         |
| 1       | Scarf       |
| 2       | Neckless    |
| 3       | Cannot see  |
| -1      | Unknown     |

### Upper Body Cloths
| Label   | Description |
|---------|-------------|
| 0       | TShirt      |
| 1       | Blouse      |
| 2       | Sweater     |
| 3       | Coat        |
| 4       | Dress       |
| 5       | Uniform     |
| 6       | Shirt       |
| 7       | Suit        |
| 8       | Hoodie      |
| -1      | Unknown     |

### Lower Body Cloths
| Label   | Description |
|---------|-------------|
| 0       | Jeans       |
| 1       | Leggings    |
| 2       | Pants       |
| 3       | Shorts      |
| 4       | Skirt       |
| 5       | Dress       |
| 6       | Uniform     |
| 7       | Suit        |
| -1      | Unknown     |

### Feet
| Label   | Description |
|---------|-------------|
| 0       | Sports Shoes |
| 1       | Classic Shoe |
| 2       | High Heels  |
| 3       | Boots       |
| 4       | Sandal      |
| 5       | Nothing     |
| -1      | Unknown     |

### Accessories
| Label   | Description     |
|---------|-----------------|
| 0       | Bag             |
| 1       | Backpack Bag    |
| 2       | Rolling Bag     |
| 3       | Umbrella        |
| 4       | Sports Bag      |
| 5       | Market Bag      |
| 6       | Nothing         |
| -1      | Unknown         |

---

## File Naming Convention

### Indoor Images
The dataset includes three types of indoor images: **F**, **L**, and **R**. The images are named according to the following convention:

```
PID_Gender_Age_Height_Weight_Ethnicity_Angle_View
```

#### Example:
```
0001_0_1_1_1_0_F.jpg
```

### Naming Components:
- **PID**: Person ID
- **Gender**:
  - Male: 0
  - Female: 1
  - Other: 2
- **Age**:
  - 0-11: 0
  - 12-17: 1
  - 18-24: 2
  - 25-34: 3
  - 35-44: 4
  - 45-54: 5
  - 55-67: 6
  - >67: 7
  - Unknown: -1
- **Height**:
  - Child (Below 150 cm): 0
  - Short (150-160 cm): 1
  - Medium (160-170 cm): 2
  - Tall (Above 170 cm): 3
  - Unknown: -1
- **Weight**:
  - Thin (Below 60 kg): 0
  - Medium (60-80 kg): 1
  - Fat (Above 80 kg): 2
  - Unknown: -1
- **Ethnicity**:
  - Indian: 0
  - Black: 1
  - Turkish White: 2
  - White: 3
- **Angle**: Camera angle
- **View**:
  - F: Front
  - L: Left
  - R: Right

### Gait Videos
The dataset also includes gait videos following the same naming convention as indoor images.

### Outdoor Images
Outdoor images follow a slightly different naming convention to capture additional details such as date, time, drone height, distance, angle, location, and other attributes.

```
PID_Date_Time_DroneHeight_Distance_Angle_Location_HairColor_HairStyle_Beard_Moustache_Glasses_HeadAccessories_UpperBodyCloths_LowerBodyCloths_Feet_Accessories_Action_DroneScene_SessionID
```

#### Example:
```
0004_23_10_2024_09_18_5.8_10_30_3_0_1_1_0_-1_-1_6_0_0_6_152_178_S1
```

### Naming Components:
- **PID**: Person ID
- **Date**: Capture date (e.g., 23_10_2024 for October 23, 2024)
- **Time**: Capture time (e.g., 09_18 for 09:18 AM)
- **DroneHeight**: Height of the drone in meters
- **Distance**: Distance in meters
- **Angle**: Angle in degrees
- **Location**: Location ID
- **HairColor, HairStyle, Beard, Moustache, Glasses, HeadAccessories, UpperBodyCloths, LowerBodyCloths, Feet, Accessories**: Encoded attributes as defined above
- **Action**: Encoded action or behavior
- **DroneScene**: Drone scene number
- **SessionID**: Session identifier

---

---

## License

# Experimental Settings Options
Experimental settings are options that do not currently have a menu option in the XboxHD+ app.
These options are stored in the settings.json configuration file (since FW2.1.6) and must be
set manually.

#### Example
```json
{
    "experimental": {
        "debug_log" : 1,
        "fanspeed"  : 5,
        "avi_infoframe": {
            "avi_info_override"                : 0,
            "picture_aspect_ratio"             : 2,
            "active_format_information_status" : 1,
            "active_format_aspect_ratio"       : 8
        },
        "boot_animation" : {
            "disable_d3d_hook" : 1,

            "io_glowcolor"     : "0x00A0FF60",
            "lipcolor"         : "0x00000100",
            "lipglow"          : "0x004B9B4B",
            "xbox_color"       : "0x0062CA13"
        }
    }
}
```

## AVI InfoFrame Override
These options allows for finer control over the AVI InfoFrames sent to the display.

---
### AVI InfoFrame Override
This must be set to 1 for the override options to be applied.

<table>
  <tr>
    <th>Field</th>
    <td>avi_info_override</td>
  </tr>
  <tr>
    <th>Type</th>
    <td>Integer</td>
  </tr>
</table>

#### Example:
```JSON
{
    "experimental": {
        "avi_info_override": 1
    }
}
```

#### Options:
| Value | Description  |
| ----- | ------------ |
|     0 | Disabled     |
|     1 | Enabled      |

---
### Picture Aspect Ratio

<table>
  <tr>
    <th>Field</th>
    <td>picture_aspect_ratio</td>
  </tr>
  <tr>
    <th>Type</th>
    <td>Integer</td>
  </tr>
</table>

#### Example:
```JSON
{
    "experimental": {
        "avi_info_override"    : 1,
        "picture_aspect_ratio" : 2
    }
}
```

#### Options:
| Value | Description   |
| ----- | ------------- |
|     0 | No Data       |
|     1 | 4:3           |
|     2 | 16:9          |

---
### Active Format Information
This must be set to 1 for 'Active Portion Aspect Ratio' to have an affect.

<table>
  <tr>
    <th>Field</th>
    <td>active_format_information_status</td>
  </tr>
  <tr>
    <th>Type</th>
    <td>Integer</td>
  </tr>
</table>

#### Example:
```JSON
{
    "experimental": {
        "avi_info_override"                : 1,
        "active_format_information_status" : 1
    }
}
```

#### Options:
| Value | Description                      |
| ----- | -------------------------------- |
|     0 | No Data                          |
|     1 | Active Format Information valid  |

---
### Active Portion Aspect Ratio
Used to communicate common “Active Format” aspect ratio information from a Source to a display device.

**Note:** ``active_format_information_status`` must be set to 1 for this to have an affect.

<table>
  <tr>
    <th>Field</th>
    <td>active_format_aspect_ratio</td>
  </tr>
  <tr>
    <th>Type</th>
    <td>Integer</td>
  </tr>
</table>

#### Example:
```json
{
    "experimental": {
        "avi_info_override"                : 1,
        "active_format_information_status" : 1,
        "active_format_aspect_ratio"       : 8
    }
}
```

#### Options:
| Value | Description                   |
| ----- | ----------------------------- |
|     8 | Same as Picture Aspect Ratio  |
|     9 | 4:3 (Center)                  |
|    10 | 16:9 (Center)                 |
|    11 | 14:9 (Center)                 |

## Boot Animation
TODO

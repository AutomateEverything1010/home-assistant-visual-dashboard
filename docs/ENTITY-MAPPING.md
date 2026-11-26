# Entity mapping

The public YAML intentionally uses neutral placeholder entity IDs. Replace each placeholder in `dashboard.yaml` with the matching entity from your own Home Assistant instance. Do not copy the placeholder literally unless you create matching entities.

| Placeholder entity | Used for |
|---|---|
| `button.replace_me_01` | chandleir drawing brighter |
| `button.replace_me_02` | chandleir drawing darker |
| `button.replace_me_03` | chandleir drawing power |
| `button.replace_me_04` | chandleir drawing warm light |
| `button.replace_me_05` | nuuk fan mode |
| `button.replace_me_06` | nuuk fan power |
| `button.replace_me_07` | nuuk fan speed |
| `button.replace_me_08` | nuuk fan swing |
| `climate.replace_me_01` | drawing ac |
| `input_boolean.replace_me_01` | away mode |
| `input_boolean.replace_me_02` | drawing chandelier |
| `input_boolean.replace_me_03` | guest mode |
| `input_boolean.replace_me_04` | nuuk fan assumed on |
| `input_boolean.replace_me_05` | nuuk lamp assumed on |
| `input_boolean.replace_me_06` | sonos speaker |
| `input_boolean.replace_me_07` | sonos speaker alert |
| `light.replace_me_01` | aquarium tube light 1 2 |
| `light.replace_me_02` | aquarium tube light 3 |
| `light.replace_me_03` | aquarium tube light 4 |
| `light.replace_me_04` | aquarium tube light 5 |
| `media_player.replace_me_01` | living room |
| `script.replace_me_01` | ac toggle |
| `script.replace_me_02` | nuuk fan power toggle |
| `script.replace_me_03` | nuuk lamp toggle |
| `sensor.replace_me_01` | aquarium water temp temperature |
| `sensor.replace_me_02` | temp ra humidity 2 |
| `sensor.replace_me_03` | temperature humidity sensor temperature 2 |
| `switch.replace_me_01` | 4sw aquarium switch 1 |
| `switch.replace_me_02` | 4sw aquarium switch 2 |
| `switch.replace_me_03` | 4sw aquarium switch 3 |
| `switch.replace_me_04` | aquarium 16a 2ch switch 1 1 |
| `switch.replace_me_05` | aquarium 16a 2ch switch 1 2 |
| `switch.replace_me_06` | below staircase |
| `switch.replace_me_07` | drawing room l2 2 |
| `switch.replace_me_08` | drawing room l3 |
| `switch.replace_me_09` | drawing room l4 |

## How to find your entity IDs

In Home Assistant, open **Settings → Devices & services → Entities**, search for the device or helper, and copy its entity ID. Replace the corresponding placeholder in the YAML. Keep the entity domain compatible with the action: for example, a `climate` entity must be mapped to your climate entity, and a `button` entity to a button entity.

The `YOUR_HA_USERNAME` value in `kiosk_mode` is also a placeholder. Replace it with the username configured in your kiosk-mode setup, or remove the `kiosk_mode` block if you do not use that feature.

### Horizontal stack

Horizontal stack card will allow you to stack together multiple cards so they always sit next to each other in the space of one column.

**Options**

| Name | Type | Default | Description
| ---- | ---- | ------- | -----------
| type | string | **Required** | `horizontal-stack`
| cards | list | **Required** | List of cards

**Example**

Basic example
```yaml
- type: horizontal-stack
  cards:
    - type: picture-entity
      image: https://images.pexels.com/photos/164595/pexels-photo-164595.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=240&w=495
      entity: light.ceiling_lights
    - type: picture-entity
      image: https://images.pexels.com/photos/545012/pexels-photo-545012.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=240&w=495
      entity: light.bed_light
```

![horizontal stacking](https://user-images.githubusercontent.com/32000001/42229254-f02b8284-7edd-11e8-9ea6-f6689e8450f5.PNG)

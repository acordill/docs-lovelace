### Vertical stack

Stack card will allow you to stack together multiple cards so they always sit together in the same column one on top of the other.  Keep in mind this can be used with any cards, and even used alongside a [horizontal-stack](card-horizontal-stack.md).

**Options**

| Name | Type | Default | Description
| ---- | ---- | ------- | -----------
| type | string | **Required** | `vertical-stack`
| cards | list | **Required** | List of cards

**Example**

Basic example
```yaml
- type: vertical-stack
  cards:
    - type: picture-entity
      entity: camera.demo_camera
      show_info: false
    - type: entities
      entities:
        - binary_sensor.movement_backyard
```

![vertical stack](https://user-images.githubusercontent.com/32000001/42230976-341c8a02-7ee2-11e8-925f-6770b86166ab.PNG)

Example using both a Vertical and Horizontal Stack Card
```yaml
- type: vertical-stack
  cards:
    - type: picture-entity
      entity: group.all_lights
      image:  https://images.pexels.com/photos/106399/pexels-photo-106399.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=750&w=1260
    - type: horizontal-stack
      cards:
        - type: picture-entity
          image: https://images.pexels.com/photos/164595/pexels-photo-164595.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=240&w=495
          entity: light.ceiling_lights
        - type: picture-entity
          image: https://images.pexels.com/photos/545012/pexels-photo-545012.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=240&w=495
          entity: light.bed_light
  ```
![vertical stack 2](https://user-images.githubusercontent.com/32000001/42231285-116cd8e4-7ee3-11e8-8ae8-aa4cdee606d2.PNG)


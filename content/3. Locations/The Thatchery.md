---
name: The Thatchery
parent_location: "[[Overworld]]"
tags:
  - location
  - kic-party
---
## Description
A quaint little restaurant, bustling and booming with business, in the middle of a small halfling village

## key info
- Founded by [[Ronda Dimplethatch]]
- Currently owned and run by [[Merla Solanum]]

### Sub-Locations
```base
views:
  - type: table
    name: Sub-Locations
    filters:
      and:
        - file.hasTag("location")
        - note["parent_location"] == this.file
    order:
      - file.name
    sort:
      - property: file.name
        direction: DESC

```
---
name: Fieldybrooke
parent_location: "[[Overworld]]"
tags:
  - location
  - kic-party
---
## Description
A small, quaint halfling town. 

## key info
The most popular restaurant there is [[The Thatchery]]

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
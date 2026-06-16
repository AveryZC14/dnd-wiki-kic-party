---
name: Thorin and Filarion's Sharehouse
parent_location: "[[Palias]]"
tags:
  - location
  - kic-party
---
## Description
A pretty cheap little sharehouse in one of the less busy parts of Palias.
It's shockingly small and cramped.
Currenly houses [[BQ]], [[Thorin Kjellsvard|Thorin]], [[Filarion Phrygia|Filarion]] and [[Bible Woman]]

## key info
Thorin and Filarion share a room

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
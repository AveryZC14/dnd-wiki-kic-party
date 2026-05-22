---
name: Ronda's House
parent_location: "[[Palias]]"
tags:
  - location
  - kic-party
---
## Description
A lovely little cottage near the outskirts of Palias. Houses [[Ronda Dimplethatch|Ronda]] and her pet cockroach [[Benee]]

## key info


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
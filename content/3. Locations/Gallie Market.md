---
name: Gallie Market
parent_location: "[[Palias]]"
tags:
  - location
  - kic-party
---
## Description
A Bustling open market with many vendors and townsfolk.

A statue of [[Gallie Ethels]] stands near the entrance, with a plaque
"In loving memory of Gallie Ethels, Great adventurer and Protector of Palias"


## key info
- 
- butcher - Grash Jawbreaker grizzled Dwarf (he/they)
	- plenty of deer meat
	- plenty of boar meat
	- Currently can't hunt as easily because there's a megaboar
	- Used to hunt with [[Gallie Ethels]]
	- loves adventurers
- Fisher - Velina Goddlepum young halfling (she/her)
	- large large fish
	- long sharp fish
	- bright scaled fish
	- Business partner with [[Boots]]
	- thinks adventurers are a mixed bag
- Farmer - Devin Stumblefoot old human (he/him)
	- Wheat, grains, milk
	- Thinks adventurers are fools. 
- [[Boots]] 
	- Selling taxidermied fish

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
        direction: ASC

```
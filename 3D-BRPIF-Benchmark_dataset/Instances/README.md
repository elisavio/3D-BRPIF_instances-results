Each instance is represented with a .json file, which is named as follows: "B{B}-R{R}-H{H}-occ_factor{occ_factor}-L{L}-F{F}-seed{seed}.json"
- B is the number of bays in the storage area
- R is the number of rows in the storage area
- H is the number of tiers per stack
- occ_factor is the percentage of occupancy of the storage area
- L is the length of the family retrieval sequence
- F is the number of different families contained in the instance
- seed corresponds to the seed used to generate it, i.e., a serial number used to identify it.

The following settings are specified in the content of the file:
- "familyRetrievalSequence" specifies the family retrieval sequence to satisfy
- "maxHeightStacks" is the number of slots per stack
- "craneBay" is the bay over which the crane is positioned at the beginning
- "craneHeight" is the height at which the crane travels along the bay- and row-directions.

Then, for every bay, the filling of each stack is given, strarting from the stack in the first row, from the lowest slot to the highest one.
# cSCM
### Simple Collection Mapping (SCM) Parser

We invented this Data Format to allow advanced Memory Transfers via Networked Sockets.

SCM or Simple Collection Mapping allows us to collect data from multiple HashMaps, lists, Queues, Stacks and other linear or non-linear datatypes and store them in a String. SCM supports multiple Datasets by nature, all included in one String Object.

Here is an example SCM Object during Advanced Handover: ```568511777281933336:3;316980441502449666:568511777281933336;568511777281933336:1;;;```

This is the Basic SCM Syntax Explained:

`:` separates a Key:Value pair. This is essentially one Hashmap or one List entry (2 Column Entry)

`,` indicates the end of a Key:Value pair (EoL Indicator). It essentially indicates a "row" in traditional Database design

`;` acts as a seperator between two Datasets (Each identified by : and ,)

`:`, `,` and `;` can be escaped to not be recognized as operational characters.

Using SCM instead of JSON can result in lower Memory Usage and Data Usage when transferring via Networked Socket, therefore reducing transferring time and allowing for a cleaner Handover.

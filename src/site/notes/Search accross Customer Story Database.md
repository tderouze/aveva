---
{"searchBox":"","industryBox":"","dg-publish":true,"permalink":"/search-accross-customer-story-database/","dgPassFrontmatter":true}
---


## Search Parameters
**Title**: `INPUT[text:searchBox]`
**Industry**: `INPUT[text:industryBox]`

## Search Results
```base
views:
  - type: table
    name: Table
    filters:
      and:
        - or:
            - this.searchBox == ""
            - file.name.contains(this.searchBox)
        - file.inFolder("AVEVA/Customer Stories")
        - or:
            - this.industryBox == ""
            - Industry.contains(this.industryBox)
    order:
      - file.name
      - Industry
    sort:
      - property: Year
        direction: DESC
      - property: file.name
        direction: ASC
    columnSize:
      file.name: 522

```
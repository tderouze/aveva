---
{"searchBox":"","industryBox":"","dg-publish":true,"keywordBox":"","permalink":"/bases-search-search-accross-customer-story-database/","dgPassFrontmatter":true}
---


## Search Parameters
**Title**:  `INPUT[text:searchBox]`
**Industry**:  `INPUT[text:industryBox]`
**Keywords**:  `INPUT[text:keywordBox]`

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
        - or:
            - this.keywordBox == ""
            - list(Keywords).map(value.contains(this.keywordBox)).contains(true)

    order:
      - file.name
      - Industry
      - Keywords
    sort:
      - property: Year
        direction: DESC
      - property: file.name
        direction: ASC
    columnSize:
      file.name: 484

```


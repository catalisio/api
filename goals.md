# Catalisio API
## Goals
### List goals
`GET /goals`
#### Description
List available goals for a site. 
#### Response body
```
[
    {
        "id" : <goal1_id>,
        "label" <goal1_label>
    },
    {
        "id" : <goal2_id>,
        "label" <goal2_label>
    }
    ...
]
```

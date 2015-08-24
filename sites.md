# Catalisio API
## Sites
### List sites
`GET /sites`
#### Description
Get list of authorised sites.
#### Response body
```
[
    { 
        "url" : <site1_url>, 
        "publicId" : <site1_publicId>
    },
    {
        "url" : <site2_url>, 
        "publicId" : <site2_publicId>
    }
    ...
]
```

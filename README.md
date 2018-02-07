# Spatial Spring

Spring Boot + Hibernate Spatial + PostGIS

## Goals
- [ ] CRUD for geospatial data (geometry as GeoJSON)
    - [x] [POST] : `/location/`
    - [x] [GET] by ID : `/location/{id}`
    - [x] [PUT] : `/location/{id}`
    - [ ] [PATCH]
    - [x] [DELETE] : `/location/{id}`
    - [x] [GET] : `/locations`
    - [x] [POST] Get locations within specified geometry (GeoJSON) : `/locations/within`
- [ ] Transform — return a new geometry with its coordinates transformed to a different spatial reference.
- [ ] Spatial Analysis (for example: Geometry buffer)

### [POST] /location/ Sample Data
```
{
    "type": "Feature",
    "properties": {
	    "name": "L"
    },
    "geometry": {
        "type": "Polygon",
        "coordinates": [
            [
                [18.5016632080, 54.5186902372369],
                [18.5009765625, 54.4488835908718],
                [18.4467315673, 54.4101394181849],
                [18.4748840332, 54.3961505667008],
                [18.5050964355, 54.4201285340543],
                [18.5085296630, 54.3369449517794],
                [18.7028503417, 54.3365446235177],
                [18.6973571777, 54.3669584638106],
                [18.5394287109, 54.3645581895214],
                [18.5339355468, 54.4245229740048],
                [18.5868072509, 54.4616571382934],
                [18.5579681396, 54.4748256848176],
                [18.5291290283, 54.4588632653735],
                [18.5270690917, 54.5194873388633],
                [18.5016632080, 54.5186902372369]
            ]
        ]
    }
}
```
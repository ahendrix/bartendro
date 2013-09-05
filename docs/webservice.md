
Web Service documentation
=========================

Web services communicate with JSON requests and replies.

Notes: 
 * There does not appear to be a call to get all available drinks yet.

`/ws/booze/match/<str>`
    Get all of the boozes matching `<str>`, where `<str>` can contain SQL wildcards
    An empty `<str>` will return all boozes

`/ws/dispenser/<int:disp>/on`
`/ws/dispenser/<int:disp>/off`
`/ws/dispenser/<int:disp>/test`
`/ws/clean`

`/ws/drink/<int:drink>`
    Make the drink with the given ID

`/ws/drink/<int:drink>/speed/<int:speed>`
    Make the drink with the given ID and speed

`/ws/drink/<int:drink>/available/<int:state>`

`/ws/drink/<int:id>/load`
    Get the drink with the specified ID

`/ws/drink/<int:drink>/save` 
        methods=["POST"]
    Update an existing drink (id != 0) or create a new one (id = 0)

`/ws/shotbot/<int:disp>`
    Dispense a shot of the booze with the given ID

`/ws/liquidlevel/test/<int:disp>`
`/ws/liquidlevel/out/<int:disp>/set`
`/ws/liquidlevel/low/<int:disp>/set`
`/ws/liquidlevel/out/all/set`
`/ws/liquidlevel/low/all/set`

`/ws/reset`
`/ws/test`
`/ws/checklevels`
`/ws/download/bartendro.db`

`/ws/options` 
    methods=["POST", "GET"]

`/ws/upload`
    methods=["POST"]

`/ws/upload/confirm`
    methods=["POST"]



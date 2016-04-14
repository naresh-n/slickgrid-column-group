### slickgrid-column-group

This plug-in is for slickgrid to group columns.

######Column Configuration : New "groupName" Property

Add a new property called "groupName" in the slickgrid column definition. Plugin used this property to group columns.

        *{id: "title", name: "Title", field: "title", width:100, groupName: "Group-1"},
        {id: "duration", name: "Duration", field: "duration", width:100, groupName: "Group-1"},
        {id: "%", name: "% Complete", field: "percentComplete", width:100, groupName: "Group-1"},
        {id: "start", name: "Start", field: "start", width:100, groupName: "Group-2"},
        {id: "finish", name: "Finish", field: "finish", width:100}*


######Features

* Plugin exposed two methods enableColumnGrouping and removeColumnGrouping.
* Auto group size when user resize columns.
* Column reorder restricted within its group.


######Example

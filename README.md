[![Build Status](https://travis-ci.org/naresh-n/slickgrid-column-group.svg?branch=master)](https://travis-ci.org/naresh-n/slickgrid-column-group)

### slickgrid-column-group

This plug-in is for slickgrid to group one level columns.

######Browser

    <link rel="stylesheet" href="../css/slick.columngroup.css" type="text/css"/>
    <script src="../src/slick.columngroup.js"></script>

######Bower
    bower install slickgrid-column-group
    
######Usage

Add a new property called "groupName" in the slickgrid column definition.

        {id: "title", name: "Title", field: "title", width:100, groupName: "Group-1"},
        {id: "duration", name: "Duration", field: "duration", width:100, groupName: "Group-1"},
        {id: "%", name: "% Complete", field: "percentComplete", width:100, groupName: "Group-1"},
        {id: "start", name: "Start", field: "start", width:100, groupName: "Group-2"},
        {id: "finish", name: "Finish", field: "finish", width:100}


        grid = new Slick.Grid("#myGrid", data, columns, options);
        plugin = new Slick.ColumnGroup()
        grid.registerPlugin(plugin);
        grid.render();
        
        plugin.enableColumnGrouping();
        
        [OR]
        
        plugin.removeColumnGrouping();
        
        
        
######Features

* Plugin exposed two methods **enableColumnGrouping** and **removeColumnGrouping**.
* Auto size applied on grouped header when user resize columns.
* Column reorder restricted within its group.


######Example
https://rawgit.com/naresh-n/slickgrid-column-group/master/examples/example-1.html

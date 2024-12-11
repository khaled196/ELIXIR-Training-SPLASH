---
title: Events
---



{% include events.html caption=false title=true event_type="upcoming_event" caption_url="/about/events" truncate=true limit=3 %}





## Tess events 

<link rel="stylesheet" property="stylesheet" href="https://elixirtess.github.io/TeSS_widgets/css/tess-widget.css"/>
<div id="tess-widget-events-table" class="tess-widget tess-widget-faceted-table"></div>
<script>
function initTeSSWidgets() {
    TessWidget.Events(document.getElementById('tess-widget-events-table'),
        'FacetedTable',
        {
            opts: {
                columns: [{name: 'Date', field: 'start'},
                    {name: 'Name', field: 'title'},
                    {name: 'Location', field: 'location'}],
                allowedFacets: ['scientific-topics', 'country', 'city'],
                facetOptionLimit: 5
            },
            params: {
                pageSize: 5,
                country: ['United Kingdom']
            }
        });
}
</script>
<script async="" defer="" src="https://elixirtess.github.io/TeSS_widgets/js/tess-widget-standalone.js" onload="initTeSSWidgets()"></script>
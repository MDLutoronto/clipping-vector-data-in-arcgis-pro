---
title: Clipping vector data in ArcGIS Pro   # Title of the page, which will be displayed in the navigation and the browser title.
layout: page  # Layout type, usually 'page' for standard pages.
nav_order: 1  # Order in the navigation menu.
description:  How to clip - cut out a piece of a dataset using another layer as a cookie cutter - vector data in ArcGIS Pro.
permalink: /  # Optional: Custom URL for the page. It will serve as the slug. For example, /home/
created_date:  # Date when the page was created. Should be in YYYY-MM-DD format.
has_children: False  # Set to True if the page has sub-pages.
staff:  # Optional: Nested list of staff members associated with the page.
  - name: Cole White  # PLACEHOLDER: Replace with actual staff member's name.
    link: https://library.utoronto.ca/staff/cole-white # link is optional
maintainer:
  - name: Cole White # PLACEHOLDER: Replace with actual maintainer's name.
    link: https://example.com/cole-white  # link is optional
# student_staff:  
# - name: Student Name
#   link: https://example.com/student-name
# - name: Another Student
#   link: https://example.com/another-student  # link is optional
---

# Clipping vector data in ArcGIS Pro

<figure>
<img src='{{ '/assets/images/clip-tool-graphic.gif' | relative_url }}' alt="
Example of subsetting spatial data by clipping" width='70%'/>
<figcaption>Image source: <a href="https://commons.wikimedia.org/wiki/File:Example_of_Clip_Tool_process.gif"
target="_blank">Wikimedia Commons</a>. <a href="https://creativecommons.org/licenses/by-sa/4.0/deed.en"
target="_blank">CC-BY-SA 4.0</a>.</figcaption>
</figure>

You may be working with a spatial vector layer that is much more geographically 
expansive than your study area. In this case, you can <b>clip</b> the layer to your
area of interest.

<b>Example:</b> This Statistics Canada layer (downloaded from
<a href="https://www12.statcan.gc.ca/census-recensement/2021/geo/sip-pis/boundary-limites/index2021-eng.cfm?year=21"
target="_blank">this page</a>), displays all census dissemination areas within
Canada. If your study area is in Eastern Canada, you may wish to clip out
a smaller portion of this layer to work with.

<a href='{{ '/assets/images/lda.png' | relative_url }}' target="_blank">
<img src='{{ '/assets/images/lda.png' | relative_url }}' alt="Canada
census dissemination area polygons" width='100%' height='100%'  style="border:
3px solid #888888;" />
</a>

• Load your large data layer into ArcGIS Pro. Open the <b>geoprocessing
toolbox</b> and search for <b>Clip</b>.

<a href='{{ '/assets/images/clip-tool.png' | relative_url }}' target="_blank">
<img src='{{ '/assets/images/clip-tool.png' | relative_url }}' alt="Analysis ->
Tools -> Clip" width='100%' height='100%'  style="border: 3px solid #888888;" />
</a>

• Specify the layer to be clipped as the <b>Input features</b>. For the <b>Clip
features</b> parameter, you can either specify an existing layer that will act
as a 'cookie cutter' on your input layer, or click the pencil icon to define
a clip area.


<a href='{{ '/assets/images/clip-tool-parameters.png' | relative_url }}' target="_blank">
<img src='{{ '/assets/images/clip-tool-parameters.png' | relative_url }}' alt="
Clip tool parameters" width='100%' height='100%' style="border: 3px solid #888888;" />
</a>

• Click <b>Run</b>. The tool will output a new, clipped layer.

<a href='{{ '/assets/images/new-clipped-layer.png' | relative_url }}' target="_blank">
<img src='{{ '/assets/images/new-clipped-layer.png' | relative_url }}' alt="
New clipped layer" width='100%' height='100%' style="border: 3px solid #888888;" />
</a>

<b>See also</b>:

• <a href="https://mdlutoronto.github.io/arcgis-pro-clipping-rasters/"
target="_blank">Clipping rasters in ArcGIS Pro<a>

• <a href="https://mdlutoronto.github.io/arcgis-pro-extracting-geographic-features-from-larger-dataset/" target="_blank">
Extracting the geographic features you need from a larger dataset in ArcGIS Pro</a>

**Technique:** [Extracting data](https://mdlutoronto.github.io/tutorials-search/?technique=Cleaning+data) \|
**Tools:** [ArcGIS Pro](https://mdlutoronto.github.io/tutorials-search/?tool=ArcGIS+Online) \|
**Data Format:** [Vector](https://mdlutoronto.github.io/tutorials-search/?dataFormat=Vector)
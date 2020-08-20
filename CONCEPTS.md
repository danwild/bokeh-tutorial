
# Notes on bokeh core concepts

- plot
  - container that holds collection of other elements, e.g. renderers, guides, tools)
- tools
  - e.g. `figure(tools='crosshair,pan,wheel_zoom,box_zoom,reset,box_select,lasso_select')`
- glyphs
  - low level visual elems, e.g. lines, circles
  - see [bokeh.models.glyphs](https://docs.bokeh.org/en/latest/docs/reference/models/glyphs.html#bokeh-models-glyphs), [bokeh.models.markers](https://docs.bokeh.org/en/latest/docs/reference/models/markers.html#bokeh-models-markers)
  - visual appearance of a glyph is tied directly to the data values that are associated with the glyph’s various attributes
- guides
  - visual aids that help users judge distances, angles - e.g. axis ticks
- annotations
  - titles, legends etc.
- ranges
  - plots generated with [bokeh.plotting](https://docs.bokeh.org/en/latest/docs/user_guide/plotting.html#userguide-plotting) will try to auto fit vis to data range with [DataRange1d](https://docs.bokeh.org/en/latest/docs/reference/models/ranges.html#bokeh.models.ranges.DataRange1d)
  - can be done manually with [Range1d](https://docs.bokeh.org/en/latest/docs/reference/models/ranges.html#bokeh.models.ranges.Range1d)
  - ranges can be shared between plots to sync them
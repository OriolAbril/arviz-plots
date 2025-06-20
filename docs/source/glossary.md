# Glossary


:::{glossary}
aesthetic
aesthetics
  When used as a noun, we use _an aesthetic_ as a graphical property that is
  being used to encode data. 

  Moreover, within `arviz_plots` _aesthetics_ can actually be any arbitrary
  keyword argument accepted by the plotting function being used.

aesthetic mapping
aesthetic mappings
  We use _aesthetic mapping_ to indicate the relation between the {term}`aesthetics`
  in our plot and properties in our dataset.

figure
  Highest level data visualization structure. All plotted elements
  are contained within a figure or its children.

EABM
  Acronym for Exploratory Analysis of Bayesian Models. We use this concept to
  reference all the tasks within a Bayesian workflow outside of 
  building and fitting or sampling a model. For more details, see the
  [EABM virtual book](https://arviz-devs.github.io/EABM/)

plot
plots
  Area (or areas) where the data will be plotted into. A {term}`figure`
  can contain multiple {term}`faceted` plots.

visual
visuals
  Graphical component or element added by `arviz-plots`

faceting
faceted
  Generate multiple similar {term}`plot` elements with each of them
  referring to a specific property or value of the data.
  
:::

## Equivalences with library specific objects

| arviz-plots name | matplotlib   | bokeh   | plotly           |
|------------------|--------------|---------|------------------|
| figure            | figure       | layout  | Figure           |
| plot             | axes/subplot | figure  | -[^plotly_plot]  |
| visual           | artist       | glyph   | trace            |

[^plotly_plot]: In plotly there is no specific object to represent a {term}`plot`.

    Instead, when adding {term}`visuals` one can choose to add a visual to all {term}`plots`
    in the {term}`figure`, or give the row/col indexes, or specify a subset of {term}`plots`
    on which to add the {term}`visual`.

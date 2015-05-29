# D3 JavaScript Network Graphs from R

Version 0.1

This is a package inspired from the work from Christopher Gandrud. 
He implemented the [d3Network](http://christophergandrud.github.io/d3Network/) package to the
[htmlwidgets](https://github.com/ramnathv/htmlwidgets) framework.

## Installation

You can install **D3forcedNetwork** from GitHub as follows:

```S
devtools::install_github('csese/D3forcedNetwork')
```

## Usage

Here's an example of `D3forcedNetwork`:

```S
# Load data
data(MisLinks)
data(MisNodes)

# Plot
D3forcedNetwork(Links = MisLinks, Nodes = MisNodes, Source = "source",
             Target = "target", Value = "value", NodeID = "name",
             Nodesize = 'size',Group = "group", opacity = 1, 
             linkDistance = 100,charge = -400, legend = TRUE,
             colourScale = "d3.scale.category20b()")
```


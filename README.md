# Using Baseliner


## Super-short Example
    <script src="baseliner.js"></script>
    <script>
    window.onload = function() {
        baseliner = new Baseliner(8);
    }
    </script>

This will add the [Baseliner](https://github.com/jkeyes/baseline/blob/master/baseliner/baseliner.js) widget to your page:

![Show Baseline](https://github.com/jkeyes/baseline/raw/master/baseliner/example_show.png)

If you click on Show Baseline an 8px baseline grid overlay is displayed:

![Hide Baseline](https://github.com/jkeyes/baseline/raw/master/baseliner/example_hide.png)

You can customize the size of the grid too:

![16px Baseline](https://github.com/jkeyes/baseline/raw/master/baseliner/example_16px.png)

## Initialisation Options

Two initialisation options are supported:

* `gridColor` — an RBGA array (`[255, 0, 0, 255]` for red) or a color string (`red`, `blue`, `green` or `grey`/`gray`). If this option is not set, it defaults to a highly transparent red.
* `gridHeight` — the height of the baseline grid. If it is not set, it defaults to 10 pixels.

## Some more examples

    // a black grid, 20 pixels high
    baseliner = new Baseliner({'gridColor': [0, 0, 0, 255], 'gridHeight': 20 });
    // a red grid, 10 pixels high
    baseliner = new Baseliner({'gridColor': 'red'});
    // a very faint grey grid, 8 pixels high

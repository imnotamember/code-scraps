# Seaborn Code Scraps

## Markers

- To fix markers that overlap/appear blurry, remove their edges by setting `linewidth=0`.
  - Example with scatterplot:

    ```python
    import seaborn as sns; sns.set()
    import matplotlib.pyplot as plt
    tips = sns.load_dataset("tips")
    ax = sns.scatterplot(x="total_bill", y="tip", data=tips)
    ```

    ![Markers with edges](https://i.stack.imgur.com/R3SD8.png)
    Versus

    ```python
    import seaborn as sns; sns.set()
    import matplotlib.pyplot as plt
    tips = sns.load_dataset("tips")
    ax = sns.scatterplot(x="total_bill", y="tip", data=tips, linewidth=0)
    ```

    ![Markers without edges](https://i.stack.imgur.com/oCIv8.png)
  - Reference(s): [SO: Remove white border from dots in a seaborn scatterplot](https://stackoverflow.com/questions/62716077/remove-white-border-from-dots-in-a-seaborn-scatterplot)
- Seaborn complains: Filled and line art markers cannot be mixed.
  - Select either [filled markers](https://matplotlib.org/stable/gallery/lines_bars_and_markers/marker_reference.html#filled-markers) or [unfilled markers](https://matplotlib.org/stable/gallery/lines_bars_and_markers/marker_reference.html#unfilled-markers).
    - Reference(s): [SO: How to add markers on legend and graph - matplotlib](https://stackoverflow.com/questions/62428351/how-to-add-markers-on-legend-and-graph-matplotlib)

# Matplotlib Code Scraps

## Markers

- To fill a space on a plot with a solid color/color overlay, use `axvspan` (fill across y-axis for x-axis range) or `axhspan` (fill across x-axis for y-axis range).
  - Example:
  
    ```python
    import matplotlib.pyplot as plt

    plt.plot(range(10))
    plt.axvspan(3, 6, color='red', alpha=0.5)
    plt.show()
    ```
  
    ![Plot with red overlay between 3 and 6 on x-axis](https://i.stack.imgur.com/Ug7RF.png)
  - Reference(s): [SO: In a matplotlib plot, can I highlight specific x-value ranges?](https://stackoverflow.com/questions/8270981/in-a-matplotlib-plot-can-i-highlight-specific-x-value-ranges)

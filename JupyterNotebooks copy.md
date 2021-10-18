# Jupyter Notebooks Code Scraps

## Plotting

### Matplotlib

- To draw vector-based plots within a notebook, insert this prior to imports:

    ```python
    %matplotlib inline
    %config InlineBackend.figure_format = 'svg'
    ```

  - Reference(s): [SO: Include output from %matplotlib notebook backend as SVG in ipynb](https://stackoverflow.com/questions/45466947/include-output-from-matplotlib-notebook-backend-as-svg-in-ipynb)

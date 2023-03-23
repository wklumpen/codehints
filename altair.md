# Altair

Here's the code hints for Altair

## Basic Plot Skeleton

```python
import altair as alt

alt.Chart(dataframe).mark_shape().encode(
    alt.X("data:Q", title="Axis Title"),
    alt.Y("text_data:N")
).properties(
    title = {
        "text": "The Main Title",
        "subtitle": "The Subtitle"
    },
    width=800,
    height=600
).configure(
    font="Atkinson Hyperlegible",
).configure_view(
    strokeWidth=0
).configure_axis(
    grid=False,
    labelFontSize=12,
    titleFontSize=14
).configure_axisY(
    labelFontWeight="bold"
).configure_title(
    fontSize=16,
    anchor="start"
)
```
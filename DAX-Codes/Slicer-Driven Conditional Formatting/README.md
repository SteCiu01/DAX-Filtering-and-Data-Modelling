# Slicer-Driven Conditional Formatting

Apply dynamic colour formatting based on slicer-driven user selections

### Simple Scenarios Templates

#### Hide/unhide a button or an object

```
Transparent_or_Blue =
IF(
  ISFILTERED(
            Dim_Table[ColumnName]
            ),
            [ColorBlue],
            [ColorTransparent]
  )
```
#### Color based on a category selection

```
Transparent_or_Blue =
IF(
  SELECTEDVALUE(Dim_Table[ColumnName]) = "Category_A",
            [ColorBlue],
            [ColorGrey]
  )
```

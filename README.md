## String


### Extract First Initial of Last Name

Aaron Bergman
```
MID([Customer Name], FIND([Customer Name]," ")+1,1)
```

### Last Name and First Initial

Aaron Bergman
```
MID([Customer Name], FIND([Customer Name]," "))+", " + LEFT([Customer Name],1)+"."
```

### Date Leve Calculation

```
CASE ([Select a Date Level])
WHEN 'Year' THEN DATENAME('year',[Order Date])
WHEN 'Quarter' THEN DATENAME('quarter',[Order Date])
WHEN 'Month' THEN DATENAME('month',[Order Date])
END
```

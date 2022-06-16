# How to calculate percentile for dataframe

```python
import pandas as pd

data = pd.DataFrame({
  'Phone': ['ip5', 'ip6', 'ip8', 'sms', 'xi'],
  'Phone Price': [204, 304, 404, 405, 305]
})

q = data['Phone Price'].quantile(0.75)
```

- `import pandas as pd` - load [lib:Pandas module](/python-pandas/how-to-install-pandas)
- `data` - will contain loaded DataFrame
- `.quantile(` - calculates specified quantile (percentile)
- `'Phone Price'` - column to calculate quantile (percentile) for
- `0.75` - will calculate 75% percentile

group: percentiles

## Example: 
```python
import pandas as pd

phoneDataSet = {
  'Phone': ['ip5', 'ip6', 'ip8', 'sms', 'xi'],
  'Phone Price': [204, 304, 404, 405, 305]
}

data = pd.DataFrame(phoneDataSet)
q = data['Phone Price'].quantile(0.75)

print(q)
```
```
404.0

```

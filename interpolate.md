# interpolate


## interpolate with linear
```
'circle-radius': [
  'interpolate',
  ['linear'],
  ['get', 'takeOff'],
  0,
  0,
  100,
  100,
],
```
              
## interpolate with outer vars
coverageRatio is outer variables
```
'line-color': [
  'interpolate',
  ['linear'],
  ['to-number', ['get', 'tripCount']],
  0,
  'rgba(0,0,0,0)',
  Math.round(30 * coverageRatio),
  '#929292',
  Math.round(60 * coverageRatio),
  '#e6da38',
  Math.round(100 * coverageRatio),
  '#00ff00',
],
```

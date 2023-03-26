# fretchart.js

## Initialization
```
<div id="chart-list"></div>

<script>
  let guitarChart = new FretChart();
  let chartEl = guitarChart.formula({ 
    fret: 'x32010', 
    finger: '321',
    name: 'C',
  });
  document.querySelector('#chart-list').append(chartEl);
</script>
```

## Properies
- fretLength `number` : clamped to minimum of 4
- scale `number`

## Methods
- FretChart() => fretChart object : initialize a new fretChart object.
- formula(`chordObject`) => canvasElement : create new chord chart canvas element.

`chordObject`
- fret `string` : character sequence of fret number [0-9](a-e) or x's and o's.
- finger `string` : character sequence of fretting hand numbering.
- name `string` : chord symbol to be printed at the bottom of chord chart

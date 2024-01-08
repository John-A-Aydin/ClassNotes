```dataviewjs
const graph = app.internalPlugins.plugins.graph
const settings = await graph.loadData()
settings.colorGroups = [
  {
    "query": "path:\"Digital Design\"",
    "color": {
      "a": 1,
      "rgb": 13382604
    }
  },
  {
    "query": "path:\"Operating Systems\"",
    "color": {
      "a": 1,
      "rgb": 13382604
    }
  },
  {
    "query": "path:\"Embedded Systems\"",
    "color": {
      "a": 1,
      "rgb": 13382604
    }
  },
  {
    "query": "path:\"Data Structures\"",
    "color": {
      "a": 1,
      "rgb": 13382604
    }
  },
  {
    "query": "path:\"Discrete Structures\"",
    "color": {
      "a": 1,
      "rgb": 3407871
    }
  },
  {
    "query": "path:Statistics",
    "color": {
      "a": 1,
      "rgb": 3407871
    }
  },
  {
    "query": "path:\"Vector Calculus\"",
    "color": {
      "a": 1,
      "rgb": 3407871
    }
  },
  {
    "query": "path:Signals",
    "color": {
      "a": 1,
      "rgb": 16771584
    }
  },
  {
    "query": "path:\"Electrical Lab\"",
    "color": {
      "a": 1,
      "rgb": 16771584
    }
  },
]
app.workspace.detachLeavesOfType('graph')
await graph.saveData(settings)
await graph.disable()
await graph.enable()
```
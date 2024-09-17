```ts
interface TreeGraphData extends NodeConfig {
  children?: TreeGraphData[]
}

const data = {
  id: 'root',
  children: [
    {
      id: 'subTree1',
      children: [...]
    },
    {
      id: 'subTree2',
      children: [...]
    }
  ]
}

const treeData = {
  id: 'root',
  label: 'root',
  children: [
    {
      id: 'subTree1',
      label: 'subTree1',
    },
    {
      id: 'subTree2',
      label: 'subTree2',
      children: [
        {
          id: 'subTree2-1',
          label: 'subTree2-1',
        }
      ]
    }
  ]
}
```

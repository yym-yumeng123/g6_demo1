```ts
interface GraphData {
  nodes?: NodeConfig[] // 节点
  edges?: EdgeCOnfig[] // 边
  groups?: GroupConfig[] // 分组
}

const data = {
  // 点集
  nodes: [
    {
      id: "node1", // String，该节点存在则必须，节点的唯一标识
      x: 100, // Number，可选，节点位置的 x 值
      y: 200, // Number，可选，节点位置的 y 值
    },
    {
      id: "node2", // String，该节点存在则必须，节点的唯一标识
      x: 300, // Number，可选，节点位置的 x 值
      y: 200, // Number，可选，节点位置的 y 值
    },
  ],
  // 边集
  edges: [
    {
      source: "node1", // String，必须，起始点 id
      target: "node2", // String，必须，目标点 id
    },
  ],
}
```

```ts
interface NodeConfig {
  id: string; // 元素的id
  shape?: string; // 元素的图形
  x?: number; // 节点的位置 x坐标
  y?: number; // 节点的位置 y坐标
  size?: number | number[]; // 节点的大小
  style?: { // 包裹样式属性的字段
    fill?: string; // 样式属性, 元素的填充色
    stroke?: string; // 元素的描边色
    lineWidth?: number; // 描边宽度
    // ...
  }
  label?: string; // 标签文字
  labelCfg?: { // 文本配置项
    position?: '' // 位置
    // ...
  }
}
```

## @superset-ui/plugin-chart-superset-ui-hello-world



This plugin provides Superset Ui Hello World for Superset.

### Usage

Configure `key`, which can be any `string`, and register the plugin. This `key` will be used to lookup this chart throughout the app.

```js
import SupersetUiHelloWorldChartPlugin from '@superset-ui/plugin-chart-superset-ui-hello-world';

new SupersetUiHelloWorldChartPlugin()
  .configure({ key: 'superset-ui-hello-world' })
  .register();
```

Then use it via `SuperChart`. See [storybook](https://apache-superset.github.io/superset-ui/?selectedKind=plugin-chart-superset-ui-hello-world) for more details.

```js
<SuperChart
  chartType="superset-ui-hello-world"
  width={600}
  height={600}
  formData={...}
  queryData={{
    data: {...},
  }}
/>
```

### File structure generated

```
├── README.md
├── package.json
├── src
│   ├── SupersetUiHelloWorld.tsx
│   ├── images
│   │   └── thumbnail.png
│   ├── index.ts
│   ├── plugin
│   │   ├── buildQuery.ts
│   │   ├── controlPanel.ts
│   │   ├── index.ts
│   │   └── transformProps.ts
│   └── types.ts
├── test
│   └── index.test.ts
└── types
    └── external.d.ts
```
# light-page

(￣ー￣) page agent

Vanilla ESM pack. Scheduler yield, WebMCP `registerTool`, Prompt API with fallback.

```js
import { createPack } from './src/index.js';

const pack = createPack({ system: 'Short answers.' });
pack.tool({
  name: 'page_outline',
  description: 'Headings on the page.',
  annotations: { readOnlyHint: true },
  execute: () => [...document.querySelectorAll('h1,h2')].map((el) => el.textContent.trim()),
});
await pack.start();
await pack.ask('page outline');
pack.destroy();
```

Runtime lives with the pack. This folder is the registry card.

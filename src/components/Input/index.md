---
nav:
  title: Components
  path: /components
---

## Input

简单演示

```tsx
import React from 'react';
import { Input } from 'react-element';
const handleChange = (e) => {
  console.log(e.target.value);
};
const defaultInput = () => (
  <Input onChange={handleChange} placeholder="随便输入点什么吧" />
);
export default defaultInput;
```

### 被禁用的 Input

```tsx
import React from 'react';
import { Input } from 'react-element';
const disabledInput = () => <Input placeholder="disabled input" disabled />;
export default disabledInput;
```

### 带图标的 Input

```tsx
import React from 'react';
import { Input } from 'react-element';
const iconInput = () => <Input placeholder="iconInput input" icon="search" />;
export default iconInput;
```

### 不同大小的的 Input

```tsx
import React from 'react';
import { Input } from 'react-element';
const sizeInput = () => (
  <>
    <Input defaultValue="large size" size="lg" />
    <Input placeholder="small size" size="sm" />
  </>
);
export default sizeInput;
```

### 带前后缀的 Input

```tsx
import React from 'react';
import { Input } from 'react-element';
const handleChange = (e) => {
  console.log(e.target.value);
};
const pandInput = () => (
  <>
    <Input
      defaultValue="prepend text"
      prepend="https://"
      onChange={handleChange}
    />
    <Input defaultValue="google" append=".com" />
  </>
);
export default pandInput;
```

<API src="./input.api.tsx">
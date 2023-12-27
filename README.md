# Stitches.dev bug demo

A simple code like:

```ts

import { styled } from '@stitches/react';

export const Button = styled('button', {
    backgroundColor: 'gainsboro',
    borderRadius: '9999px',
    fontSize: '13px',
    padding: '10px 15px',
    '&:hover': {
        backgroundColor: 'lightgray',
    },
});


```

Leads to this error:

```
error TS2742: The inferred type of 'Button' cannot be named without a reference to '../node_modules/@stitches/react/types/css-util'. This is likely not portable. A type annotation is necessary.
```

@see: https://github.com/stitchesjs/stitches/issues/1055

# handy-snippets| Zustand
![How to Use](https://github.com/gyeongseokKang/handy-snippets/assets/61446585/3d84b401-dd9d-48ec-a0b2-9428a00bc87c.gif)

## Features

1. provides zustand snippet(prefix -zs) with typescript, middleware(persist, devtools, immer)

## Snippets

### Export Default Components

| Snippet | Renders                             |
| ------- | ----------------------------------- |
| `edc`   | export default component            |
| `edcp`  | export default component with props |
| `edf`   | export default function             |

### Zustand Stores

> Note: `persist`, `devtools`, and `immer` are from the official libraries, while `history` is implemented using Zundo.

To use `immer`, you need to download the `immer` library, and for `history`, you need to download `zundo`.

| Snippet | Renders                                     |
| ------- | ------------------------------------------- |
| `zs`    | zustand store                               |
| `zsp`   | zustand store with persist                  |
| `zsd`   | zustand store with devtools                 |
| `zsi`   | zustand store with immer                    |
| `zspi`  | zustand store with persist, immer           |
| `zsdi`  | zustand store with devtools, immer          |
| `zsdpi` | zustand store with devtools, persist, immer |
| `zsh`   | zustand store with history                  |
| `zsih`  | zustand store with immer, history           |
| `zspih` | zustand store with persist, immer, history  |

## Market Place
go to [Market Place](https://marketplace.visualstudio.com/items?itemName=handy-kang.handy-snippets).  

## Rule(원칙)

1. Use lowercase letters only | 소문자만을 사용한다.
1. Combine the first letters of the word. | 단어의 첫문자들을 조합한다. export default component => edc

## Example(예시)

```json
{
  "export default component": {
    "prefix": "edc",
    "body": [
      "const ${1:${TM_FILENAME_BASE}} = () => {",
      "  return <>$2</>;",
      "};",
      "",
      "export default ${1:${TM_FILENAME_BASE}};"
    ],
    "description": "export default component"
  }
}
```

## TIP

[snippet generator](https://snippet-generator.app/?description=export+default+function&tabtrigger=edf&snippet=const+%24%7B1%3A%24%7BTM_FILENAME_BASE%2F%28.*%29%2F%24%7B1%3A%2Fpascalcase%7D%2F%7D%7D+%3D+%28%29+%3D%3E+%7B%0A++return%3B%0A%7D%3B%0A%0Aexport+default+%24%7B1%3A%24%7BTM_FILENAME_BASE%7D%7D%3B&mode=vscode)

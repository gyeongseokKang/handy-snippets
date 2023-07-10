# handy-snippets| Zustand

[VSC 마켓](https://marketplace.visualstudio.com/items?itemName=handy-kang.handy-snippets).  
![handy-snippets](https://user-images.githubusercontent.com/61446585/216868415-278ae7c9-afc3-4794-809d-af9953f979a3.gif)

## Features

1. provides zustand snippet(prefix -zs) with typescript, middleware(persist, devtools, immer)

## Snippets

| Snippet | Renders                                     |
| ------- | ------------------------------------------- |
| `edc`   | export default component                    |
| `edcp`  | export default component with props         |
| `edf`   | export default function                     |
| `zs`    | zustand store                               |
| `zsp`   | zustand store with persist                  |
| `zsd`   | zustand store with devtools                 |
| `zsi`   | zustand store with immer                    |
| `zspi`  | zustand store with persist, immer           |
| `zsdi`  | zustand store with devtools, immer          |
| `zsdpi` | zustand store with devtools, persist, immer |

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

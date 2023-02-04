# handy-snippets| 내가 만든 나만의 스니펫 모음집

내가 편하려고 만든 코드 스니펫 모음

## Features

1. zustand + typescript에 대한 기본 생성 스니펫 제공

## Snippets

| Snippet | Renders                           |
| ------- | --------------------------------- |
| `edc`   | export default component          |
| `edf`   | export default function           |
| `zs`    | zustand store                     |
| `zsi`   | zustand store with immer          |
| `zsip`  | zustand store with immer, persist |

## 원칙

1. 소문자만을 사용한다.
1. 단어의 첫문자들을 조합한다. export default component => edc
1. 설명은 조합되는 문자열을 작성한다.

## 예시

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

## 팁

스니펫 템플릿 생성
[snippet generator](https://snippet-generator.app/?description=export+default+function&tabtrigger=edf&snippet=const+%24%7B1%3A%24%7BTM_FILENAME_BASE%2F%28.*%29%2F%24%7B1%3A%2Fpascalcase%7D%2F%7D%7D+%3D+%28%29+%3D%3E+%7B%0A++return%3B%0A%7D%3B%0A%0Aexport+default+%24%7B1%3A%24%7BTM_FILENAME_BASE%7D%7D%3B&mode=vscode)

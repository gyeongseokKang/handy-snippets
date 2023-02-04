# handy-snippets README

This is the README for your extension "handy-snippets". After writing up a brief description, we recommend including the following sections.

## Features

Describe specific features of your extension including screenshots of your extension in action. Image paths are relative to this README file.

For example if there is an image subfolder under your extension project workspace:

\!\[feature X\]\(images/feature-x.png\)

> Tip: Many popular extensions utilize animations. This is an excellent way to show off your extension! We recommend short, focused animations that are easy to follow.

## Requirements

If you have any requirements or dependencies, add a section describing those and how to install and configure them.

## Extension Settings

Include if your extension adds any VS Code settings through the `contributes.configuration` extension point.

For example:

This extension contributes the following settings:

- `myExtension.enable`: Enable/disable this extension.
- `myExtension.thing`: Set to `blah` to do something.

# handy_snippet | 내가 만든 나만의 스니펫 모음집

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

# Word Dictation

一个用于英语单词听写和拼写练习的纯前端网页应用。打开 `index.html` 即可使用，无需安装依赖。

## 功能

- 支持纸质模式：自动朗读词单，结束后显示完整答案。
- 支持在线模式：听单词后输入拼写，自动判断正误。
- 支持导入 `.txt` 和 `.json` 词单。
- 支持语速、朗读间隔、重复次数设置。
- 支持重听、跳过、暂停、继续、结束和打乱顺序。
- 自动去重并保存最近一次导入的词单到浏览器本地存储。
- 适配桌面端和移动端浏览器。

## 词单格式

TXT 文件可使用换行、逗号或分号分隔：

```txt
apple
banana
computer, dictionary; education
```

JSON 文件支持字符串数组：

```json
["apple", "banana", "computer"]
```

也支持对象数组，对象中可使用 `word`、`en` 或 `text` 字段：

```json
[
  { "word": "apple" },
  { "en": "banana" },
  { "text": "computer" }
]
```

## 使用方法

1. 用 Chrome、Edge 或 Safari 打开 `index.html`。
2. 点击“导入词单”，选择 `.txt` 或 `.json` 文件。
3. 选择“纸质模式”或“在线模式”。
4. 根据需要调整语速、间隔和重复次数。
5. 点击“开始听写”。

## 浏览器兼容

本项目使用浏览器内置的 Web Speech API 进行语音朗读。建议使用最新版 Chrome、Edge 或 Safari。

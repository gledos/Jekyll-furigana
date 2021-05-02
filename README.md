# Jekyll-furigana

[![Latest release](https://img.shields.io/github/release/gledos/Jekyll-furigana.svg?style=flat-square&logo=github)](https://github.com/gledos/Jekyll-furigana/releases/latest)
![license](https://img.shields.io/github/license/gledos/Jekyll-furigana?style=flat-square)
![language](https://img.shields.io/badge/language-liquid-orange.svg?style=flat-square&logo=markdown)
![made with <3](https://img.shields.io/badge/made%20with-%3C3-red.svg?style=flat-square&logo=githubsponsors)

GitHub Pages compatible transcription templates (furigana) without plugins or JavaScript, Use only liquid template language.

无需 jekyll 插件或 JavaScript 实现的 GitHub Pages 标音(furigana)效果，仅使用 liquid 模板语言

## Usage

1. Download the `furigana.html` file from [the master branch](/furigana.html).
2. Move file to your `_includes` folder.
3. Like the code below, use this template:

```liquid
{% include furigana.html text="测试" furigana="test" %}
{% include furigana.html text="测,试" furigana="cè,shì" type="B" %}
```

## Parameters

This snippet is highly customizable. Here are the available parameters to change the behavior of the snippet.

| Parameter  |  Type  |    Default    | Description                                                              |
| ---------- | :----: | :-----------: | ------------------------------------------------------------------------ |
| `text`     | string |   "no_text"   | Text in Kana or Chinese characters to be annotated                       |
| `furigana` | string | "no_furigana" | Hiragana, romanization or other transcription; shown above the Base text |
| `class`    | string |    "null"     | a CSS class to the <ruby> tag                                            |
| `type`     | string |      "A"      | single word single furigana                                              |
|            |        |               | when input "B": more word more furigana                                  |

## Performance

The performance impact of this code snippet on your website is negligible. The following statistics are from Jekyll's `--profile` option.

```text
| Filename                                   | Count |    Bytes |  Time |
---------------------------------------------+-------+----------+--------

# A total of 732 Phonetic in Version 0.1.0
| _includes/furigana.html                    |   732 |   47.98K | 0.054 |
```

## License

This snippet may be redistributed under either the [MIT](https://github.com/gledos/jekyll-furigana/blob/master/LICENSE) licenses.

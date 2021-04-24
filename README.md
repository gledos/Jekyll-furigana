# Jekyll-furigana

GitHub Pages compatible transcription templates (furigana) without plugins or JavaScript.

## Usage

1. Download the `furigana.html` file from [the master branch](/furigana.html).
2. Move file to your `_includes` folder.
3. Like the code below, use this template:
zhen
```liquid
{% include furigana.html text="测试" furigana="test" %}
```

## Parameters

This snippet is highly customizable. Here are the available parameters to change the behavior of the snippet.

| Parameter  |  Type  |    Default    | Description                                                              |
| ---------- | :----: | :-----------: | ------------------------------------------------------------------------ |
| `text`     | string |   "no_text"   | Text in Kana or Chinese characters to be annotated                       |
| `furigana` | string | "no_furigana" | Hiragana, romanization or other transcription; shown above the Base text |
| `class`    | string |    "null"     | a CSS class to the <ruby> tag                                            |

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

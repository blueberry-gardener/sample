
subtitle
<div style="font-size: 250%;">
文章について
</div>
<div style="text-align: right;">
2023-1-11<br>
XXXX
</div>

---



# 目次

- [目次](#目次)
- [Markdownの整理](#markdownの整理)
  - [Markdownの整理](#markdownの整理-1)
  - [画像](#画像)
  - [style.less](#styleless)
  - [いいい](#いいい)
  - [うう](#うう)
    - [ううう](#ううう)
- [Markdown Preview](#markdown-preview)




# Markdownの整理

こんな感じで作っていく。さｈだｋｈかｓｄｈｋだｓｈｋｊｄさｈかｈｄｓｋじゃｓｄｈｋｊｄｋｄｈはｄｓｋだｓｋだｋはｋｄｈｋだｈｄ。

こんな感じで作っていく。さｈだｋｈかｓｄｈｋだｓｈｋｊｄさｈかｈｄｓｋじゃｓｄｈｋｊｄｋｄｈはｄｓｋだｓｋだｋはｋｄｈｋだｈｄ。

## Markdownの整理
こんな感じで作っていく。さｈだｋｈかｓｄｈｋだｓｈｋｊｄさｈかｈｄｓｋじゃｓｄｈｋｊｄｋｄｈはｄｓｋだｓｋだｋはｋｄｈｋだｈｄ。

sjadjalsdjlajdadsklasjlakdsjlda

- MarkdownPreviwEnhancedを入れる(Yiyi)
- MarkDown All in One
- `Ctrl+Shift+P`で`Markdown Preview Enhanced : Customize CSS`


<div>
<b>参考文献</b><br>
https://qiita.com/UKawamura/items/42f907c88686fb3be4da <br>
https://www.ipride.co.jp/blog/5007
</div>


## 画像
```html
<img width="数値" alt="代替テキスト" src="URL">
```

## style.less

```json

/* Please visit the URL below for more information: */
/*   https://shd101wyy.github.io/markdown-preview-enhanced/#/customize-css */
body{
  counter-reset: chapter;
  font-family: "メイリオ","游ゴシック";
}

h1{
  counter-reset: sub-chapter;
  font-family: "メイリオ","游ゴシック";
}

h2{
  counter-reset: section;
  font-family: "メイリオ","游ゴシック";
}

h3{
  counter-reset: sub-section;
  font-family: "メイリオ","游ゴシック";
}

h4{
  counter-reset: sub-sub-section;
  font-family: "メイリオ","游ゴシック";
}

p,li {
  text-indent: 1em;
  font-size: 10pt;
}

.markdown-preview.markdown-preview {
  h1::before{
    counter-increment: chapter;
    content: counter(chapter) ". ";
  }

  h2::before{
    counter-increment: sub-chapter;
    content: counter(chapter) "." counter(sub-chapter) ". ";
  }

  h3::before{
    counter-increment: section;
    content: counter(chapter) "." counter(sub-chapter) "." counter(section) ". ";    
  }

  h4::before{
    counter-increment: sub-section;
    content: counter(chapter) "." counter(sub-chapter) "." counter(section) "." counter(sub-section) ".";    
  }

  h5::before{
    counter-increment: sub-sub-section;
    content: counter(chapter) "." counter(sub-chapter) "." counter(section) "." counter(sub-section) "." counter(sub-sub-section) ".";    
  }
}

```

## いいい

```powershell
$env:http_proxy="http://ssss"
```

## うう

### ううう

```bash
envsss=aaa 
curl -L $envsss
```

# Markdown Preview

https://h-s-hige.hateblo.jp/entry/20190405/1554467885

```
{
    "folders": [
        {
            "path": "vscode_workspace"
        }
    ],
    "settings": {
        "markdown.preview.fontFamily": "'MigMix 1M', 'Yu Gothic', 'Meiryo', 'SFUIText-Light', 'HelveticaNeue-Light', sans-serif",
        "markdown.preview.fontSize": 16,
        "markdown.preview.lineHeight": 1.8,
        "markdown-pdf.styles": [
            "./markdown-pdf.css"
        ],
        "markdown-pdf.margin.top": "3cm",
        "markdown-pdf.margin.bottom": "2.2cm",
        "markdown-pdf.printBackground": true,
        "markdown-pdf.displayHeaderFooter": true,
        "markdown-pdf.headerTemplate": "<div style=\"position: relative; margin-top: 0.5cm; margin-bottom: 0.5cm; margin-left: 1cm; margin-right: 1cm; width: 100%;\"><img style=\"height: 48px;\" src=\"data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAPAAAAB2CAMAAAG2Zd7zAAAAS1BMVEUAAAAtUbYvT7ctUbEvT7MvT7ItUbMuUbMvT7QvUbMuUrQuUbUvULQvULMuUbQvULQuUbMuUbQuUbQvULMvULMuUbQvULQvULMvUbTRrKeAAAAAGHRSTlMAHCA4QFBUWGCAj5+rt7/Hz9vf4+fv8/eJW3VfAAAClElEQVR42u2cfVuDIBTFHVlpFi02F9//k/Zs60UU8HJBFDu/P/as8Ho4goBXXVUtjjYoUYCHEOJeI3HFusXMDlasvHkYW//hbseRnSeaUGwItO5q1f5a1+My9fNdGiUNrfhgNOik2FEJSnHWhvXQhvWKyt2MtqCuzGAbdcyB8gTr7srl9mmv9FmNeTI11SREeurSJAyejlp68WDjSBz+NlAenipAGAzm5zde948IJlSXpYzgxToJq3OUFnwftr9R1i2mw5B1v4qmrPcRfFsYi2F/Er8QlXVg4xUabO86MxMd5reyZtyopfmsMO9qsiDhdkQ24fHJ3AlWGIQhvGFhathRmjS5hOsqkn8hbE4r9YCHpYVdC0bHQkUyp8omWpjXQhAeCQ9HgU9ppZ/+K16YsvzgnnIQXlHYiUi61s6ekwcA3OYM7jlbsDArrIPwdoXHmYg+l3CiTswRZk36EsIQhjCEIZxs8A4XpiH1+Eo9m3B0fg3CEN6FsDt7u7Tw8BGH4R+XAGFFwJs9cuY1FxhGw4VnJwlac0AYwnsXnr8zMF1uyD5eWAw4ObPJE+KFCXmIZBMJhCEM4XTCgZdeOtUKJPTRPsWlAgAAAPYL+x7vag9txxvO+A5xB8MwDMMw7Icwbj7XCdmC4c7Lh37tknHWWzA8V4eEXVrCMAzDMAzDMAzDMAzD8LAOCdfSR+0vf9uA4cc2IWr9FE/eH7STOv5lVhiGYRiGYRgu33DjYq+GOXd5VOGGHSXOt+UCnxd5kQT6dDfdmrUNS8sDhBPeKRuR9rMFw6k2op0aMAzDMAzDMLxTw1lZ37ATFXQrPPuafBHDAQlaGIZhGIZhGIbhIMOhF9mnUMMiH6QEAIMww3nBD/QBAIrnC8vt+gzmA2P4AAAAAElFTkSuQmCC\" /></div>",
        "markdown-pdf.footerTemplate": "<div style=\"font-family: 'MigMix 1M', '游ゴシック体', 'Yu Gothic', YuGothic, 'ヒラギノ角ゴ Pro', 'Hiragino Kaku Gothic Pro', 'メイリオ', 'Meiryo', sans-serif; position: relative; color: #202020; border-top: 1px solid #202020; margin-top: 0.5cm; margin-bottom: 0.5cm; margin-left: 1cm; margin-right: 1cm; font-size: 9px; width: 100%;\"><div style=\"position: absolute; width: 100%; top: 0.3cm; text-align: center;\"><span class='pageNumber'></span> / <span class='totalPages'></span></div></div>"
    }
}
```

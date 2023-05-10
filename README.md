# my-report-template


MarkDownでレポートを書きたいし、なんかいい感じにしたいっていうモチベーションで作ったテンプレートです。
いまはKumassyさんの[Qiita](https://qiita.com/Kumassy/items/5b6ae6b99df08fb434d9
)を参考にさせていただいています。

settings.jsonはまだできてるけどできてません。

ビルド(WSL)
```
docker run -it --rm -v `pwd`:/workspace -v `pwd`:/root/.pandoc/templates kumassy/alpine-pandoc-ja pandoc -F pandoc-crossref report.md -o report.pdf --pdf-engine=lualatex --template mytemplate.tex -N
```
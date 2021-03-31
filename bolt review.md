
# 見た目
## header
- position:fixed; で固定+[top:0;left:0;]で角固定する：ブラウザによっては、変な所に配置されてしまうため
- PC,TAB版の時は [display:none;] でハンバーガーメニューを非表示にする：見えていなくても、”０”で表示されているため
- display:none; で消した要素は[display:block;]で表示させる
## クラス名
- sectionとarticleはタグに依存しているため、固有のものに変える：他のタグに置き換えることがあるため（ただしnavigationは例外のため、クラス名に使ってもいい）
[section→introduction]<br>[article→collection]
## what we can do
- 画像とテキストの間はタイトル(introduction-title)ではなく、それをまとめているクラス(introduction-text)のmarginで取る方が適切
## our latest work
- nth-childの見直し：3つ区切りにしたい場合、今のまま(nth-child(+4))だと７枚目を追加した時３枚目の下についてしまうため:[nth-of-child(4n)]で指定
# コード
## html
- metaタグ：descriptionとkeywordの追加
- 28行目にaタグの消し忘れ
## css
- 今回はpcサイトから作ったため、pc版の指定はグローバルに当てて、spとtab用は必要な箇所にだけ指定する。また、spとtabの指定はほとんど同じのため、[max-width:1199px]でまとめる。
- ４００行くらいにまとめられたらOK！
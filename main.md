---
marp: true
theme: default
style: |
  @import url('theme.css')
paginate: true
header: "Marp入門"
footer: "© 2024 yuya"
---

<!-- タイトルスライド -->
# Marp入門
## Marp初心者がまとめる、Marpの使い方基礎

氏名: Yuya
日付: 2024年7月28日


---

<!-- 目次スライド -->
# 目次

## 1. 自己紹介
## 2. Marpって何？
## 3. Marpのできること、できないこと
## 4. まとめ

---

<!-- 自己紹介スライド -->
<div class="split-flex ml-50">
<div class="left-60per mr-50">

<div>
    <img class="icon" src="./my-icon.png" alt="アイコン">
</div>

<div class="info">

##  Introduction
- 年齢: 25歳
- 職業: プログラマ
- 出身: 福岡県
- 好きな食べ物: 刺身🐟・コーヒー☕️

</div>

<div class="quote">

"最近、趣味を増やしたいと悩んでます..."

</div>
</div>

<div class="right-40per ml-50">

# <span class="name"><u>Name: Yuya Inoue</u></span>

<div class="hobbies">

## Hobbies
- Fishing 🎣
- アプリ開発 💻

</div>

<div class="languages">

## Favorite languages
1. TypeScript
2. Python
3. C# 

</div>

</div>
</div>

---

<!-- タイトル2 -->
# Marpとは？

---

<!-- Marpとは？ - description -->
#  Marpとは？


## Markdown記法を用いてスライドが作れちゃう便利ツール

- アプリがVSCode**１つで**完結
- うまく利用すれば**メモがそのままスライドに！**
- エンジニアなら**コーディング感覚で**スライドを作成できちゃう！
- CSS・HTMLも利用できるので**カスタマイズ性が高い**
- **統一性**が出る

---

# Marpでできること・できないこと

---

<div class="split-flex ml-50">
<div class="left-50per">

# <u>できること</u>

<div>

- コーディング感覚で資料作成
- md記法でスライドが作れる
- VSCodeで資料作成できる
- CSSでカスタマイズ

</div>
</div>
<div class="split-50per">
<div>

# <u>できないこと</u>

</div>
<div>

- そもそもGUI使えない...
- 複雑な図形を作れない
- そもそもmd記法が必要
- 細かな調節にHTML・CSS必要


</div>
</div>
</div>

---

# 便利そうだけど、コーディングするのめんどくね？
## そもそもわい、CSS苦手...

---

# 最強の味方AIに書いてもらおう！
### 指示は俺に任せろ！
と、いうことでこれからテキトーにmdでメモをとったファイルを投げて実際に作ってみます。

---

# 生成AIを使って試しに作ったスライド

---

<!-- タイトルスライド -->
# React SuspenseとNext.js Loading UI
## 効果的なローディング表示の実装

---

<!-- Suspenseの説明 -->
# Suspenseとは？ {.split-flex}

<div class="left-50per">

![height:300px](https://react.dev/images/docs/illustrations/i_suspense.png)

</div>

<div class="right-50per">

- React 18から正式サポート
- 子コンポーネントの読み込み完了まで
  フォールバックUIを表示
- 使い方は簡単：Suspenseでラップするだけ

</div>

---

<!-- Suspenseの使用例 -->
# Suspenseの使用例

```typescript
import { Suspense } from 'react';

function MyComponent() {
  return (
    Loading ...}>
      
    
  );
}
```

詳細: https://ja.react.dev/reference/react/Suspense

---

<!-- Loading UIの説明 -->
# Next.js Loading UIとは？ {.split-flex}

<div class="left-50per">

![height:300px](https://nextjs.org/_next/image?url=%2Fdocs%2Flight%2Floading-special-file.png&w=1920&q=75)

</div>

---

# 思ったよりちゃんとできてしまった。。。

クラス名が出てたりと多少、手直しが必要そうな部分はあるがこれだけちゃんと出力してくれれば全然OKだと僕は思っています。

何より僕はスライドを作るのが苦手だし、嫌いなのでこれはかなり使える！

(生成したスライドに少し手直しを加えたフルバージョンとプロンプトは同じリポジトリ内にあるので興味のある方は見てみてください)

---

# まとめ

---

# まとめ
- Marpはmdでスライドが作成できるツール
- HTML・CSSを用いれば、高いカスタマイズ性
- VSCodeの拡張機能でプレビューを見ながら作成できる
- AIを組み合わせることで爆速でスライドができる

## 僕みたいにスライド作成・CSS嫌いエンジニアには最高の手法だと思ってます
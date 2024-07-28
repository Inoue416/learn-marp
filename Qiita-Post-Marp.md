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
# React SuspenseとNext.js Loading UI
## 効果的なローディング表示の実装

---

<!-- Suspenseの説明 -->
# Suspenseとは？

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
# Next.js Loading UIとは？ 

<div class="left-50per">

![height:300px](https://nextjs.org/_next/image?url=%2Fdocs%2Flight%2Floading-special-file.png&w=1920&q=75)

</div>

<div class="right-50per">

- Next.js 13から導入
- App Routerと併用
- コンポーネントごとにカスタマイズ可能なローディング表示
- Suspenseと連携して動作

</div>

---

<!-- Loading UIの使用方法 -->
# Loading UIの使用方法

1. `app`ディレクトリ直下に`loading.tsx`を作成
2. ローディング中に表示したいUIをコンポーネントとして実装
3. 必要に応じて、サブディレクトリにも`loading.tsx`を配置してカスタマイズ

```typescript
// app/loading.tsx
export default function Loading() {
  return Loading...;
}
```

---

<!-- ディレクトリ構造の例 -->
# ディレクトリ構造例 {.split-flex}

<div class="left-40per">

```
app
├── App1
│   └── page.tsx
├── App2
│   ├── loading.tsx
│   └── page.tsx
├── layout.tsx
├── loading.tsx
└── page.tsx
```

</div>

<div class="right-60per">

- ルートの`loading.tsx`はデフォルトのローディングUI
- `App2`ディレクトリ内の`loading.tsx`は
  そのルート専用のカスタムローディングUI
- Next.jsが適切なローディングUIを自動的に選択

</div>

---

<!-- 実装例 -->
# 実装例：カスタムローディングUI

```typescript
// app/App2/loading.tsx
export default function Loading() {
  return (
    
      Loading App2...
    
  );
}
```

Next.jsは、`App2`ルートでこのカスタムローディングUIを使用します。

---

<!-- まとめ -->
# まとめ

- **Suspense**:
  - React 18の機能
  - コンポーネントのローディング状態を簡単に管理
- **Next.js Loading UI**:
  - App Router専用機能
  - ルートごとにカスタマイズ可能
  - Suspenseと連携して動作

両機能を組み合わせることで、
ユーザーエクスペリエンスを大幅に向上させることができます。

---

<!-- 参考リンクとサンプルコード -->
# 参考リンク・サンプルコード {.split-flex}

<div class="left-50per">

## 公式ドキュメント
- [React Suspense](https://ja.react.dev/reference/react/Suspense)
- [Next.js Loading UI](https://nextjs.org/docs/app/building-your-application/routing/loading-ui-and-streaming)

</div>

<div class="right-50per">

## サンプルコード
GitHubリポジトリ:
[Learn-NextJs-LoadingUI](https://github.com/Inoue416/Learn-NextJs-LoadingUI)

実際の実装例を確認できます！

</div>

---

<!-- 終了スライド -->
# ご清聴ありがとうございました

効果的なローディング表示で、
アプリケーションのUXを向上させましょう！
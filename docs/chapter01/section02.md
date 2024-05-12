# Angular の概要

複数のプラットフォームを利用できるアプリを Web 技術で作るためには、「SPA」（Single Page Application）という
単一ページで構成する手法で開発します。

SPA では、`example.com/user` や、`example.com/detail` といった URL への遷移を行いますが、
ブラウザが読み込む HTML ファイルは `index.html` の1つです。

コンテンツの中身を JavaScript で書き換えて、まるでページ遷移したように表示するのです。  
コンテンツだけではなく URL も JavaScript で書き換えます。

## 特徴① HTML / CSS / TypeScript を分けて書く

### Angular の場合

```typescript
@Component({
    templateUrl: './angular.component.html', // ここで HTML を呼び出し
})
export class WelcomeComponent {
    message: string = 'Hello World!'
}
```

```html
<div>{{message}}</div>
```

### Vue.js の場合

HTML の中に Script を書きます。

```html
<div id="app">
    {{ message }}
</div>
<script>
    const app = new Vue({
        el: '#app',
        data: {
            message: 'Hello World!'
        }
    })
</script>
```

### React の場合

JSX と呼ばれる拡張記法を使って、JavaScript で HTML の構造を書きます。

```typescript jsx
ReactDOM.render(
    <h1>Hello, world!</h1>,
    document.getElementById('root')
)
```

## 特徴② All in One パッケージ

Angular はエコシステムが充実しています。

## 特徴③ セマンティックバージョニングとアップデート

Angular は CLI にアップデート機構（ng update）を搭載しており、メジャーバージョンリリースで API のは快適変更があった場合、
そのアップデート機構が API のは快適変更に追随したコードの変更を自動的に行なってくれます。

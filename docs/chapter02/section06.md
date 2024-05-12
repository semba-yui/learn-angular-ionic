# プロジェクトを作ろう

## コマンド一つで自動生成

```shell
ionic start --type=angular
```

ログ

```shell
$ ionic start --type=angular

Every great app needs a name! 😍

Please enter the full name of your app. You can change this at any time. To bypass this prompt next time, supply name,
the first argument to ionic start.

? Project name: tasklist-tutorial

Let's pick the perfect starter template! 💪

Starter templates are ready-to-go Ionic apps that come packed with everything you need to build your app. To bypass this
prompt next time, supply template, the second argument to ionic start.

? Starter template: sidemenu
? Would you like to build your app with NgModules or Standalone Components? 
 Standalone components are a new way to build with Angular that simplifies the way you build your app. 
 To learn more, visit the Angular docs:
 https://angular.io/guide/standalone-components

 NgModules
[INFO] Existing git project found (/Users/semba/ghq/github.com/semba-yui/learn-angular-ionic). Git operations are
       disabled.
✔ Preparing directory ./tasklist-tutorial in 687.96μs
✔ Downloading and extracting sidemenu starter in 659.56ms
> ionic integrations enable capacitor --quiet -- tasklist-tutorial io.ionic.starter
> npm i --save -E @capacitor/core@latest

added 1180 packages, and audited 1181 packages in 1m

203 packages are looking for funding
  run `npm fund` for details

found 0 vulnerabilities
> npm i -D -E @capacitor/cli@latest

added 58 packages, and audited 1239 packages in 6s

207 packages are looking for funding
  run `npm fund` for details

found 0 vulnerabilities
> npm i --save -E @capacitor/haptics @capacitor/app @capacitor/keyboard @capacitor/status-bar

added 4 packages, and audited 1243 packages in 7s

207 packages are looking for funding
  run `npm fund` for details

found 0 vulnerabilities
> capacitor init tasklist-tutorial io.ionic.starter --web-dir www
✔ Creating capacitor.config.ts in /Users/semba/ghq/github.com/semba-yui/learn-angular-ionic/projects/tasklist-tutorial in 3.07ms
[success] capacitor.config.ts created!

Next steps: 
https://capacitorjs.com/docs/getting-started#where-to-go-next
[OK] Integration capacitor added!

Installing dependencies may take several minutes.

  ──────────────────────────────────────────────────────────────────────────────

         Ionic Advisory, tailored solutions and expert services by Ionic

                             Go to market faster 🏆
                    Real-time troubleshooting and guidance 💁
        Custom training, best practices, code and architecture reviews 🔎
      Customized strategies for every phase of the development lifecycle 🔮

                        👉  https://ion.link/advisory  👈

  ──────────────────────────────────────────────────────────────────────────────


> npm i

up to date, audited 1243 packages in 749ms

207 packages are looking for funding
  run `npm fund` for details

found 0 vulnerabilities

Join the Ionic Community! 💙

Connect with millions of developers on the Ionic Forum and get access to live events, news updates, and more.

? Create free Ionic account? No

Your Ionic app is ready! Follow these next steps:

- Go to your new project: cd ./tasklist-tutorial
- Run ionic serve within the app directory to see your app in the browser
- Run ionic capacitor add to add a native iOS or Android project using Capacitor
- Generate your app icon and splash screens using cordova-res --skip-config --copy
- Explore the Ionic docs for components, tutorials, and more: https://ion.link/docs
- Building an enterprise app? Ionic has Enterprise Support and Features: https://ion.link/enterprise-edition
```

| テンプレート名      | 概要                           |
|:-------------|:-----------------------------|
| tabs         | シンプルなタブのテンプレート               |
| sidemenu     | サイドメニュー（ハンバーガーメニュー）のあるテンプレート |
| blank        | blankページを表示するテンプレート          |
| my-first-app | 公式チュートリアル用テンプレート             |
| conference   | Ionicの実装デモンストレーション           |

## プレビューを起動して開発を始めよう

```shell
ionic serve
```

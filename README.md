# expo-minimal-template

### up

```bash
yarn dev
```

### build

```bash
eas build -p [platform] -e [enviroment]
eas build -p android -e development
```

`Android` は動作確認ずみ  
`iOS` は Apple Developer account が必要なので確認していない  

`development` は devClient build が作成され、開発時 local server に繋いでに使用する  
`preview` を動作確認で使う  

### submit

```bash
eas submit -p [platform]
```

## 事前準備

- eas-cli のインストール
  - https://docs.expo.dev/build/setup/
  - https://github.com/expo/eas-cli
  - docker で環境作れば、local に入れなくても良いのだが...
- expo のアカウント作成
  - https://expo.dev/
- expo のプロジェクトを作成
  - 作成したら`eas init --id xxxxxxxxxx`
  - これで`app.json`の`projectId`が更新される
 
## Expoについて
- `eas build` はt 30回/month まで無料
- native module を更新した場合、`devClient`をビルドし直す必要がある

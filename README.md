# org-secrets-scan
`aquasecurity/trivy`を使用して秘匿情報を検出し。Pull Request にコメントを追加します。

この workflow は [Required workflows](https://docs.github.com/ja/actions/using-workflows/required-workflows) の機能を用いて GLOBIS Organization 配下の全てのリポジトリで動作されることを前提としています。

![image](https://github.com/globis-org/org-secrets-scan/assets/35423021/e5127c69-a45b-4024-99fd-4a646a67a8d1)


## カスタマイズ
必要に応じて、各リポジトリのルートディレクトリに `trivy-secret.yaml` を配置することで検知ルールの追加や検知対象から外すことができます。

詳細は [公式ドキュメント](https://aquasecurity.github.io/trivy/v0.48/docs/scanner/secret/#configuration) を参考にしてください

`trivy-secret.yaml` が意図したように動くかはローカル環境で動作確認することが可能です。

trivy のインストール方法については [こちら](https://aquasecurity.github.io/trivy/v0.48/getting-started/installation/) を参考にしてください。

# GitHub において、2段階認証をしていても git push をする方法
* 参考: [Githubの2段階認証入れたらpushできなくなった人へ - Qiita](https://qiita.com/cyborg__ninja/items/6efd349370bf5f8bffb2)  

まず、Personal Access TokenをGitHubの設定画面から生成する。  
次に、一度 `git push` をし、パスワードを要求された時に生成したトークンを入力する。

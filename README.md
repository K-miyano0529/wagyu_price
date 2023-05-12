# Git Lesson

## リモートリポジトリとローカルリポジトリとはそれぞれ何でしょうか？
* そもそもリポジトリとは、データなどを納める箱のようなもので、この文脈ではソースコードが保管されている場所。
* リモートリポジトリは、ネット上のリポジトリのこと。
* ローカルリポジトリとは、PCごとのリポジトリのこと。


## プッシュとマージの違いは何でしょうか？
* プッシュとは、ローカルからリモートへとデータの変更履歴を反映させる作業のこと。
* マージとは、各ブランチで行った作業を幹ブランチに合わせる作業のこと。


## コミットとプッシュの違い
* コミットとは、ローカルで行っていた作業の変更履歴をブランチに登録をする作業のこと。
* プッシュとは、ローカルでコミットした内容をリモートに対して登録する作業のことをいう。


## コミットのメッセージはどのように書いてあげるのが最適でしょうか？
* 一目見ただけで、変更の内容が分かるように書くことが最適。


## ローカルでマージするフローと、プルリクエストでマージするフローの違いは何でしょうか？
* ローカルでマージすると、その幹ブランチをそのままリモートにプッシュした場合、自分だけで完結してしまい、すべてが合わさる本番環境で、予期せぬバグが起こる可能性がある。
* プルリクエストでマージすると、自分の担当するブランチに対してpushをしているだけで、幹ブランチに直接は関与せず、プルリクエストでレビューアーを通すことで、バグの発生などを最小限に留めることが可能。


## コンフリクトを起こしてしまった場合、どう対処すべきですか？
1. 最初にマージされていたものを適応する。
2. 後からマージされていたものを適応する。
3. どちらの変更内容も適応させる。
* どれを選択するかは状況によって異なるので、その場その場での判断が必要。
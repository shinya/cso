# slackのスタンプをカウントするアプリ
## 事前設定
* main.pyと同じフォルダにlocal.pyを作成する
* local.py内に定数を記述する
	```
	#投稿先のチャンネル名
	CHANNEL_NAME = "#random"
	#OAuth Access Token
	USER_TOKEN = "xoxp-xxxx-xxxx-xxxx-xxxx"
	#Bot User OAuth Access Token
	BOT_TOKEN = "xoxb-xxxx-xxxx-xxxx"
	```
* slack APIでBOTに割り当てる権限
	* chat:write
	* users:read
* slack APIでUSERに割り当てる権限
	* channels:history
	* channels:read
	* groups:read
	* im:read
	* mpim:read
## 実行方法
* pythonでmain.pyを実行してください。
	```
	python main.py
	```
## 投稿イメージ
* 表示件数等の変更は、const.pyの数値を変更してください。
	```
	2020年11月22日のスタンプランキングを発表します。
	このスタンプが良く使われました:+1:
	1位 :おだんご: 3
	2位 :ハロウィーン: 2
	3位 :爆笑: 1
	このユーザーがたくさんスタンプしました:+1:
	1位 Aさん 3
	2位 Bさん 2
	3位 Cさん 1
	```

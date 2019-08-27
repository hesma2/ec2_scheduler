## AWS EC2のスケジューリング起動
### ファイル構成
#### config/ec2_connection.txt
- EC2インスタンスの接続情報

#### src/ec2_control.sh
- EC2インスタンスの起動停止を行う
- cron等のスケジューラを用いることで、スケジューリング設定が可能
- 複数インスタンスの制御は未実装
　→　複数の場合、txtファイルよりもJsonファイルの方が良さそう
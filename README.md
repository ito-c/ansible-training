# ansible-training

docker の ansible でターゲットに apache をインストールするまで

## 起動

```bash
$ docker-compose build --no-cache
$ docker-compose up -d
$ docker-compose exec ansible bash
```

## 疎通確認

管理サーバーからターゲットへの疎通確認

```bash
$ ansible node -m ping
```

## 実行

```bash
$ ansible-playbook playbook.yml
```

# cobbler-server
make the Cobbler server at Vagrant + Ansible

## 使用したbox
https://github.com/momijiame/packer-vanilla-box
cent > 6をPackerしたもの

```bash
$ packer build -only=virtualbox-iso centos6.json
```

## 手順メモ
1. $ vagrant box add CentOS6.6 作成したbox
2. $ vagrant init CenOS6.6
3. $ githubからVagrantfileとansibleのファイルを落とす
4. $ vagrant up
5. $ vagrant ssh
6. つながる

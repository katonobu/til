# 鍵生成@20230302
- 元ネタ:[(初心者)SSLソケット通信](https://qiita.com/butada/items/9450e39d8d4aac6ac1fe)
- [オレオレ証明書・秘密鍵・CSR全部まとめて作るワンライナー](https://qiita.com/marcy-terui/items/2f63d7f170ff82531245)
  - `openssl req -nodes -newkey rsa:2048 -keyout server.key -out server.csr -subj "/C=JP/ST=Hokkaido/L=Sapporo/O=Example INC./OU=IT Department/CN=example.com" && openssl x509 -req -days 3650 -in server.csr -signkey server.key -out server.crt`

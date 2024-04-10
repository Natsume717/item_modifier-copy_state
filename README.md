# item_modifier-copy_state
item_modifierの1項目であるcopy_stateのサンプルになります。

詳しくはブログ記事『[【マイクラ】copy_stateでブロックの情報をコピー【item_modifier】](https://natsumake.com/item_modifier-copy_state/)』を参考にしてください。

<h3>使い方</h3>

データパック導入後、ワールドに入ることで

+ かまど
+ 溶鉱炉
+ 石炭
+ 鉄の原石
+ ダイヤモンドのツルハシ

が付与されます。

これらを使って、燃焼中のかまど、溶鉱炉を壊すことで、copy_stateが適用されたアイテムを入手することが可能です。<br>
※燃焼中でなくとも問題ありません。燃焼中であればlit=true、燃焼中でなければlit=falseという結果になります。

ブロック破壊後は入手したアイテムをメインハンドに持って、以下のコマンドを実行しましょう。
tagがコピーされているかどうか確認することができます。

```copy
/data get entity @s SelectedItem
```

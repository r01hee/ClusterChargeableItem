# Cluster Creator Kit Sample Plus

Cluster Creator Kit を用いた Unity プロジェクトです。  

[Cluster Creator Kit Sample](https://github.com/ClusterVR/ClusterCreatorKitSample)からForkして、Logicを組み合わせて作ったアイテムのサンプルシーンをプラスしています。

Cluster Creator Kitの正しい使い方で実装できているか分からないため、あくまで実装の一例であることをご理解ください。  

## Usage

[Cluster Creator Kit Sample](https://github.com/ClusterVR/ClusterCreatorKitSample) からForkしたプロジェクトなので、導入方法などはそちらをご覧ください。

`Assets/ClusterCreatorKitSamplePlus/Scenes`内にこのプロジェクトで追加したサンプルシーンがあります。

## Samples

### ChargeableItem

`Assets/ClusterCreatorKitSamplePlus/Scenes/ChargeableItem.unity`

時間でカウントが溜まり、その溜まったカウント数に応じて段階的に性能が変わる(時間でチャージできる)ようなアイテムの実装の一例です。  

アイテムを使うと、  
30%未満: 発射不可  
30〜59%: 小ボール発射  
60〜99% 中ボール発射  
100% 大ボール発射  
となるサンプルです。  

![chargeable-item-demo](https://raw.githubusercontent.com/wiki/r01hee/ClusterCreatorKitSamplePlus/images/chargeable-item-demo.gif)


### ExchangeableItem

`Assets/ClusterCreatorKitSamplePlus/Scenes/ExchangeableItem.unity`

アイテムを使うことで、そのアイテムの性能や見た目を切り替えることができるサンプルです。  
ダメージを与える(与えられる)アイテムと、ダメージを与えられたらしばらく無敵時間になりその間はダメージを受けなくなるアイテムのサンプルも兼ねてます。  

アイテムを使うと 短い棒->長い棒->先が広い長い棒->短い棒... と順番に切り替わる候補が表示され、アイテムを離すことで切り替わりが確定します。  

![exchangeable-item-exchange-demo](https://raw.githubusercontent.com/wiki/r01hee/ClusterCreatorKitSamplePlus/images/exchangeable-item-exchange-demo.gif)

アイテムのそれぞれの与えられるダメージ(攻撃力)は 短い棒:3, 長い棒:2, 先が広い長い棒:1 に設定されています。  
アイテムを持ってキューブに当てるとキューブにダメージが加算されていきます。  
キューブはダメージを受けると色が変わり無敵時間となり、その間はダメージを受けなくなります。  
一定時間経過するとキューブの色は戻り無敵時間が終了し、再度ダメージを受ける状態に戻ります。  

![exchangeable-item-damage-demo](https://raw.githubusercontent.com/wiki/r01hee/ClusterCreatorKitSamplePlus/images/exchangeable-item-damage-demo.gif)

## LICENSE

`Assets/ClusterCreatorKitSamplePlus/`内についてはCC0  

([Cluster Creator Kit Sample](https://github.com/ClusterVR/ClusterCreatorKitSample) のオリジナル部分に関してはオリジナルに準じます。)  

[![CC0](http://i.creativecommons.org/p/zero/1.0/88x31.png "CC0")](http://creativecommons.org/publicdomain/zero/1.0/deed.ja)

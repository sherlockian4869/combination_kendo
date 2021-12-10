# トーナメント表自動生成

選手の出身チームと過去の対戦履歴を考慮した対戦表を自動で生成する  

## トーナメント表作成メモ
人数を考慮して4つの山に分ける  
例：選手が12人だった場合→12÷4=3  
　　1つの山に3人いることになる  
    <img src="/image/12人トーナメント.png" width="500px">  
　　選手が29人だった場合→29÷4=7...1  
    1つの山に7人×3と8人の山ができる  
    <img src="/image/29人トーナメント.png" width="500px">  

## 考慮すること
LEVEL00 データ作成  
LEVEL01 1回戦の相手は出身チーム以外の組み合わせ  
LEVEL02 ベスト4まで出身チームとできるだけ合わないような組み合わせ  
LEVEL03 過去の対戦履歴から1度当たったことのなる相手とは1回戦で当たらない  
LEVEL04 昨年度の大会の結果を踏まえて、ベスト4に入った選手が四隅に配置  
LEVEL05 LEVEL04を踏まえて、2回戦で同じチーム同士で当たらない  

[選手名簿](https://drive.google.com/drive/u/2/folders/17o9UglqI12nPJLFZ7HobPLn8ZplH98Gd)

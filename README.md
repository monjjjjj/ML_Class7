# ML_Class7
## Adversarial Attack: Basic Concepts
1. Network在一班的情況下得到高的正確率是不夠的，必須在就算是有人蓄意欺騙他的時候還能維持高正確率！
2. 類神經網路光是正確率高還不夠，我們希望他能應付來自人類的惡意攻擊
## Adversarial Attack: Attack and Defense
1. Black-box attack: 如果我們不知道訓練資料的時候怎麼辦？只要拿一堆資料，放到model裡，得到output之後，就拿到成對的資料了，再把此成對資料拿去訓練模型，就有可能訓練出一個proxy network！
2. 黑箱攻擊在non-target attack比較容易成功，target attack比較不容易成功！
3. 有一群人主張：攻擊會成功，主要的問題來自data而非模型，因為不同模型訓練出來的結果是相近的！當有足夠的資料，有可能就能避免攻擊！
4. 主動防禦：一開始就訓練一個比較不會被攻破的模型->Adversarial Training（不斷地找漏洞，再去補漏洞），就算沒人要攻擊，也能用此方法來減少overfitting的狀況發生
   被動防禦：：模型已訓練好，模型不動，在模型前面加一個filter(如smoothing)，去削減attack signal的威力！
## Explainable AI: Why Does the Model Make This Prediction (機器為何可以得到正確答案？)
1. 需要機器學習的模型是具有解釋力的！如醫療診斷理由、銀行是否貸款給某個人、法官判案、自駕車急煞的理由等
2. 真正用的技術不是單棵decision tree，而是decision forest！ -> 所以並不是有decision tree就能解決explainable ML problem
3. Explainable ML的目標是什麼？
   (1)能夠了解模型的一切？但我們也不理解腦袋運作的一切，但我們仍相信腦袋所做的決定！所以我們需要了解模型的一切嗎？
   
   (2)人能接受的理由，就是好的理由，所以我們才需要ML Model需要可以被解釋
## Explainable AI: Why Does a Cat Look Like (for a Model)

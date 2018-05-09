
## new data についてプロジェクトのながれ


1.前処理：  
new_data.xlsx => [New_FA] =>   
New_edu_data.txt (重要)    
New_edu_data_pre.txt  
New_id_to_wd.pickle   
New_wd_to_id.pickle   
New_wd_set.pickle  
New_id_to_lb.pickle  



2.学習と予測：   
New_edu_data.txt => [New_XXX(ラベル)_svm] =>     
New_pred_Epistemic_data_X.txt  
New_pred_Argumentation_data_X.txt  
New_pred_Coordination_data_X.txt  
New_pred_Social_data_X.txt  

3.相関係数を得るための前処理：   
New_pred_Epistemic_data_X.txt  
New_pred_Argumentation_data_X.txt  
New_pred_Coordination_data_X.txt  
New_pred_Social_data_X.txt  をまとめて => new_pred_X.xlsx


new_pred_X.xlsx => [New_pred2result] => temp.csv => new_result_X.xlsx  


3.相関係数の計算：    
new_result_X.xlsx => [New_Valuation_X] => new_table_X.xlsx















































## タグについての話
### タグの付け方
稲葉先生の"A framework to analyze argumentative knowledge construction in computer-supported collaborative learning"という論文から

### epistemic
- On task  
問題解決に取り組んでいるか
- Off task  
取り組んでいないか

### coordination
Off Taskのときのみにつく(はず)
- Task division  
誰が出す、私が提出するなどの主張や、誰がどれを行うかなど
- Time management  
時間進行
- Technical coordination  
提出完了（システムに干渉）共有のまとめ　システムを介して
- Quote  
引用文、URLなど
- Proceedings  
議事進行
- 空欄  
どのタグにも属さない場合

### argumentation
- Simple Claim  
単なる主張-学習者の意見を根拠、限定なく提示　例（感じ、maybe、提示、同意を求めるなど)
- Qualified Claim  
限定付きの主張-ある環境下でのみその主張が正しいということを明言　
- Grounded Claim  
根拠をもった主張-主張を正当化（warrant)する根拠(grounds)を持つ主張 　例(〜であるため、〜である）
- Grounded and Qualified claim  
限定付きかつ根拠をもった主張
- Non-argumentative moves  
非議論的発言（質問も含む）

### social
- Externalization  
外化：他者の発言への参照なく発言 (Target は無記入で良い）
- Elicitation  
情報の引き出し：質問によって他者の発言を求める (Target は無記入で良い）
- Quick consensus building  
早急な合意形成：納得することなく他者の発言を受けいれる
- Integrarion-oriented consensus building  
統合を目指す合意形成：相異なる意見を参考に自身の意見を検討
- Conflict-oriented consensus building  
対立を目指す合意形成：他者の発言の特徴点を特定し、それを修正したり、別の解決策や見方を提示する必要がある
- Summary  
グループの発言をまとめたもの、総合的な発言の結果
- 空欄  
どのタグにも属さない場合,No Sense で意味不明な場合

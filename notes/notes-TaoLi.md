Notes  
===============
Notes for slide:  
Experiments & Observational Studies: Causal Inference in Statistics

Basic Concepts  
---------------
1. Causal Inference  
	相关性不代表因果关系，相关性可能由hidden bias导致。slides里面的例子, 处理乳腺癌的两种疗法: 切除+化疗, 只是切除没有化疗。
2. Observational Studies
	与experiment是相对的，observational存在问题:Fundamental Problem of Causal Inference (FPCI),即对每个unit在一个时间只能观测一个结果。
3. Experiments Studies
	随机化实验。下面的RCM成立在假设之下：Stable Unit Treatment Value Assumption (SUTVA), 即每一个unit的potential outcome和这个unit接受的treatment没有关系。
4. Rubin Causal Model
	在SUTVA下，考虑potential outcomes, 求平均因果作用(average causal effect, ACE)。	 

Main Methods
-------------
1. Fisher exact test
	实质上是超几何分布，检验treatment和control是否相同。
2. Wilcoxon signed rank test
	检验treatment和control是否相同。先求差值，再对两个组分别计算差值序列的秩和。
3. Propensity score matching
	

To-do List
------------
- [ ] sensitivity analysis
- [ ] pattern specification

Questions
------------
to be done...

Reference
-----------
1. [Experiments & Observational Studies: Causal Inference in Statistics](http://www-stat.wharton.upenn.edu/~rosenbap/ExperAndObsTalk.pdf)  
2. [Wikipedia: Propensity score matching](https://en.wikipedia.org/wiki/Propensity_score_matching)
3. [Wikipedia: Rubin causal model](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=1&ved=0CB0QFjAA&url=http%3A%2F%2Fen.wikipedia.org%2Fwiki%2FRubin_causal_model&ei=YljPU6ThFcSHogT4oYHwBg&usg=AFQjCNF-oYhUtYxHBzDrWvJBphi7411EpA&sig2=A3c3V1OatGlFZxwr-78-iQ&cad=rjt)

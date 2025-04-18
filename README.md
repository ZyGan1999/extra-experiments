# Extra Experiments

## Larger LLMs
**Caption:** We have conducted extra experiments on larger LLMs including Qwen2.5-14B-Instruct and Qwen2.5-32B-Instruct, with the same setting as results in Fig.2 of our main text. 
<img src="Larger-LLMs/larger-llms.png" alt="larger-llms" />
## Analysis by Difficulty
**Caption:** We have conducted extra experiments to analyze the mutual information (MI) and accuracy by different difficulty levels. The experiments are performed on MATH-500, where the questions are divided into 5 different difficulty levels (level 1 for the simplest, level 5 for the most difficult). The questions at the same level share similar difficulty. 
**(a) The MI analysis by difficulty levels.** We present the relationship between the estimated MI and average response length at different levels. For all 5 levels, we observe similar MI decay phenomena like Fig.2 in our main text. 
**(b) The accuracy analysis by difficulty levels.** We present the relationship between the average accuracy and the length of responses at different levels. For all 5 levels, we observed that accuracy generally decreases with response length. Furthermore, the accuracy of the simplest level 1 decreases significantly when length increases, demonstrating the harm of overthinking. 
<img src="Analysis-by-Difficulty/analysis-by-difficulty.png" alt="analysis-by-difficulty" />

## Influence of $k$
**Caption:** We have conducted extra experiments to further verify Theorem 4.6 by examining the influence of $k$. The experiments are performed on GSM8k and PrOntoQA, and we vary the value of the "max-action" of an MCTS while keeping other hyperparameters optimal, according to previous studies. The results illustrate that: (1) the reasoning correctness increases when the reasoning cost $k$ increases; (2) for simpler PrOntoQA task where the value function is more reliable, the accuracy increases faster than GSM8k when $k$ increases. 
<div align="center">
<img src="Influence-of-k/influence-of-k.png" alt="influence-of-k" style="width: 50%;"/>
</div>

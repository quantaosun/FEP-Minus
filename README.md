
## Here comes FEP-Minus

The calculation logic is the same as the FEP-Plus, so the accuracy is the same.

This notebook can allow you directly run an FEP calculation in the free Google Colab (Free, at least at the time this was created, but I know things are getting weird since Colab decided to count hours now to force you to pay for GPU).


A typical calculation for a protein with 300 to 400 amino acids could finish within 8 hours with a Tesla V100. 


[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/quantaosun/FEP-Minus/blob/main/FEP-Minus.ipynb)



## Pre-condition. Apply Desmond from the D.E.Shaw research group.

## FEP-Minus can also be run on any cloud platform with a good GPU. The only thing you need to change is the ```USER``` environment variable of that platform when you compile the software to that platform. 

### For users from China, you may want to have a look at my project on AI Studio where generously provide each user 8 hour V100 GPU every day. 
- notebook 版本： https://aistudio.baidu.com/aistudio/projectdetail/4311927?contributionType=1 
- 脚本任务 版本：   https://aistudio.baidu.com/aistudio/clusterprojectdetail/4309423
- 建议使用脚本任务版本，免费算力时间更长，运行更稳定，不容易中断

## Something you need to keep in mind

As with any other method, FEP has its limitation as well. There are three situations you shouldn't use this methodology.

The binding pocket is highly flexible or changes greatly upon binding to the ligand.

The two ligands share a similarity of less than 60%.

*The two ligands bind to the pocket in quite different modes, even though they share greater than 60% chemical similarity.*

Note 60% is my personal view of a similarity boundary, you could argue it could be 70% or 50%.

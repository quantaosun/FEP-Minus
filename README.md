
## Here comes FEP-Minus

The calculation logic is the same as the FEP-Plus, so the accuracy is the same.

This notebook can allow you directly run an FEP calculation in the free Google Colab (Free, at least at the time this was created, but I know things are getting weird since Colab decided to count hours now to force you to pay for GPU).


A typical calculation for a protein with 300 to 400 amino acids could finish within 8 hours with a Tesla V100. Suppose you can not use the free GPU from Google Colab, which is volatile over time to time, user to user. Please consider spend the money of a cup (or two/three) of coffee to buy some GPU hours. It is nothing compared to your cost for each job using commercial software.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/quantaosun/Install_and_Run_Desmond_Academic_FEP_on_Colab/blob/main/Run_Desmond_ligand_FEP_on_colab.ipynb)

## Pre-condition. Apply Desmond from the D.E.Shaw research group.

## FEP-Minus can also be run on any cloud platform with a good GPU, the only thing you need to change is the ```USER``` environment variable of that platform when you compile the software to that platform.

## Motivation and backgroud of this project

As of 2022, FEP calculation is still of high value and the commercial price is expensive. This notebook is to provide the academic and non-profit research community with a real solution if they want to try this new method. There are way too many so-called FEPs that take forever to learn and finish. Desmond is the fastest and most reliable one I have ever met, with GPU supported, a typical FEP could be finished with 10h, with a Tesla V100 on Google Colab, with only a subscription fee of around 70 USD per month. It is a bit expensive if you look at it from a coffee price way, but it is nothing compared to some commercial FEP license fee. It is guaranteed the academic version is working, For the commercial version, I have not tested it yet, you may need to adjust some of the commands, or it might be not possible if the commercial one fixes the IP address but Colab allocates us random IP every time.

This is for an FEP simulation, input files are produced from the Desmond Academic Maestro LigandFEP module. Written by quantaosun@gmail.com in 2021, Shanghai, China, during the leave from my PhD program. The ultimate goal here is to allow you to calculate the difference in free energy of binding between a pair of small molecules. This is the first of its kind that properly introduce how to run this kind of complicated simulation with Free GPUs from Colab to the best of my knowledge.

## Something you need keep in mind

As any other methods, FEP has its limitation as well. There are three situations you shouldn't use this methodology

The binding pocket is highly flexible or changes a lot upon binindg to ligand.

The two ligands share a similarity less than 60%.

The two ligands binds to the pocket in quite different modes, even they share greater than 60% chemical similarity.

Note 60% is my personal view of a similarity boundary, you could argue it could be 70% or 50%.

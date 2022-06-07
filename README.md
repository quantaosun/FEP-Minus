# Install_and_Run_Desmond_Academic_FEP_on_Colab
One of the most reliable free FEP (Academic) for med chem inhibitor optimisation, one to rule them all.

# 1. Apply Desmond from D.E.Shaw research group.
# 2. Install it on a platform allow you to use GUI (Maestro) to prepare your FEP input files.
# 3. Upload another copy of installer package and the FEP files to Colab. (You can click the button bellow to open)
# 4. Adjust the file names to yours in the colab notebook, and run the simulation, wait it to finish.


[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/quantaosun/Install_and_Run_Desmond_Academic_FEP_on_Colab/blob/main/Run_Desmond_ligand_FEP_on_colab.ipynb)


If you use AI Studio https://aistudio.baidu.com/aistudio , please set "USER" to "aistudio"

As of 2022, FEP calculation is still of high value and the commercial price is expensive. This notebook is to provide the academic and non-profit research community with a real solution if they want to try this new method. There are way too many so-called FEPs that take forever to learn and finish. Desmond is the fastest and most reliable one I have ever met, with GPU supported, a typical FEP could be finished with 10h, with a Tesla V100 on Google Colab, with only a subscription fee of around 70 USD per month. It is a bit expensive if you look at it from a coffee price way, but it is nothing compared to some commercial FEP license fee. It is guaranteed the academic version is working, For the commercial version, I have not tested it yet, you may need to adjust some of the commands, or it might be not possible if the commercial one fixes the IP address but Colab allocates us random IP every time.

As any other methods, FEP has its limitation as well. There are three situations you shouldn't use this methodology

The binding pocket is highly flexible or changes a lot upon binindg to ligand.
The two ligands share a similarity less than 60%.

The two ligands binds to the pocket in quite different modes, even they share greater than 60% chemical similarity.

Note 60% is my personal view of a similarity boundary, you could argue it could be 70% or 50%.

下面是一个快速的中文简介

![image](https://user-images.githubusercontent.com/75652473/172171197-218b3201-2316-4492-87fb-a8a1e516fb9a.png)




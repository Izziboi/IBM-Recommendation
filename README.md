# IBM-Recommendation
## Introduction<br>
This project aims to make recommendations to IBM Watson Studio platform users. Users of this platform have user ids and there are thousands of articles to access. Each article has an article id and a name. Users access articles as much as they want. As they access the articles, the plaform keeps track of the number of interactions. All these information are contained in the datasets used for this project. The essence of this work is to recommend articles for users based on certain conditions such as the articles their statistical neighbors have interacted with. Neighbors in this context, are users who have accessed some of the articles a particular user has accessed. There are also other conditions implemented in the analyses as can be seen in the codes of the work. The codes have docstrings that explain what each function does and can be understood by a non programmer.<br>
## Python Modules Used<br>
The python modules used in this work include:<br>
- pandas<br>
- numpy<br>
- matplotlib<br>
- pickle<br>
## Files and Folders In the Repository<br>
Below are the various folders and files in the repository:<br>
**- articles_community.csv and user-item-interactions.csv:** These are the datasets from the IBM Watson Studio platform, for analyses.<br>
**- Recommendations_with_IBM.ipynb:** This is the jupyter notebook file containing the codes of this project. The .html version is also included and is designated Recommendations_with_IBM.html.<br>
**- project_tests.py:** This is a python file containing some codes used to test some of the codes of this project.<br>
**- top_5.p, top_10.p and top_20.p:** These are other test codes used to test another section of the codes of this project.<br>
**- user_item_matrix.zip:** This is a zip pickle file of a matrix version of the dataset. This dataset presents the users and the articles they interacted with. The users are the index rows while the articles are the columns and the interactions are denoted with 1s while non-interactions are denoted with 0s.<br>
## How To Run The Program<br>
It is easy to run this program. The codes are arranged in functions with docstrings explaining their tasks. One can choose any function of choice, input the necessary parameter and run to see the result. Therefore, the program can be run in parts. On the other hand, one can input the necessary parameters to all the functions run simultaneously, to see the various results.<br>
## Results<br>
**- Part I : Exploratory Data Analysis:** This part is concerned with exploration of the datasets analyzed in this project. Below is an example of the type of results shown in the part.<br>
![part_one](https://user-images.githubusercontent.com/44449730/153963381-f6095d8d-e85c-4815-a07e-cb3003f7060b.jpg)
<br>
**- Part II: Rank-Based Recommendations:** This part produces the high ranking articles which is a function of the number of times the user has interacted with articles. Below is a typical result from this section - showing article name and their ids.<br><br>
![part_two](https://user-images.githubusercontent.com/44449730/153964039-b901ae95-9283-4435-9637-535fd94003f2.jpg)
**- Part III: User-User Based Collaborative Filtering:** This portion makes recommendations by showing articles a neighbor has read which a user has not yet read. Below is a result from there - showing names of articles of that type.<br><br>
![part_four](https://user-images.githubusercontent.com/44449730/153964701-8e030e7d-432b-48c8-a5dc-f036284929da.jpg)
<br>
**- Part V: Matrix Factorization:** This part uses Single Value Decomposition (SVD) to make recommendations. Below is a result from the part.<br><br>
![part_five](https://user-images.githubusercontent.com/44449730/153965032-d4f27659-9db9-41bb-9dcc-ec898cfd6af9.jpg)

## Summary<br>
The above listed parts are the functional parts of the project codes. One can decide which technique to use for recommendation. Whatever choice made, the appropriate part and function may be consulted and deployed to get the expected result.<br>
## Acknowledgement<br>
I sincerely appreciate the IBM Watson Studio for providing us with the datasets for this project. It is a very good contribution to the success of this course. I also thank the Udacity team, more especially the Mentors, for their sound lectures and attention to questions. Their technical assistance can simply be described as unquantifiable because without it, completing this project would have been extremely difficult. Please accept my heart-felt gratitude.<br>
## References<br>
1. https://classroom.udacity.com/nanodegrees/nd025/parts/d5affd42-242c-4f3c-9394-3bb0530c96d4/modules/d0bb49fe-9492-4897-9101-0ed957313461/lessons/b92da9ee-e204-4a0c-b5a7-b801d534088a/concepts/7d302bb6-ce2a-43d2-84e2-2c702171655c<br>
2. https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.unstack.html<br>


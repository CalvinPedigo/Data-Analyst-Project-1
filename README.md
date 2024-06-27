# Data-Analyst-Project-1
Our project aims to answer one simple question. Is lane splitting safer for motorcycles? To answer this we accessed the NHTSA's FARS crash data, and registration data provided by IIHS both found in the Resources Folder. To answer this question, we broke it up into smaller pieces; we decided that some of the best things to determine what could make or break the safety of lane splitting was to look at a couple variables that go into these reports. We looked at motorcycle type, the laws of the state, the resulting injury severity, and the death rates for the states that allow them.

Only a handful of states have laws allowing motorcycle splitting or filtering, and we used these states that correlate with the data we had at the time. California allows full lane splitting, being anywhere that has 2 lanes of traffic following the same direction. States like Utah and Hawaii allow lane filtering (meaning when traffic is stopped), and of course the majority of states either do not allow splitting, or do not have any laws stating so.

Our analysis began with the csv files that we had on hand, and we sorted and filtered the unimportant bits out. We then proceeded to organize what was important into years, states, injuries, deaths, engine size, lanes, etc. We primarily coded with python, using some dependencies like pandas, scipy, mattplotlib, and a few other libraries to help us out. Using these we made many different dataframes, graphs, charts, and functions to get the data we need to answer our questions. After all is said and done, we have come to our conclusions.

Time to answer our original question: Is lane splitting safer for motorcycles? While there are many different factors that go into an individual crash, only a few get reported. It's important to note this fact, as it may not paint the entire picture, or paint the wrong picture entirely. That beind said, our data shows there are less injuries and fatal crashes in states where lane splitting is legal or somewhat legal. While the differences are not large, these findings were consistent throughout. Using statistical tests, however, the only difference that was deemed significant was the increase of fatal crashes in states where laws are not mentioned. Since, there are so many factors in a motorcycle crash we also looked at a couple of variables that could skew and alter our conclusion. States where laws were not mentioned also had increases in driving without a helmet and drunk driving crashes. While our findings implicate that there is a correlation between  motorcycle safety and not mentioned lane splitting laws, possible confounding variables make it difficult to draw any causation. Another, interesting aspect of multiple lane motorcycle crashes that we explored was differences based of motorcycle type. We found that there was a significant increase in the number of crashes large motorcycles were invovlved in, which implicates another factor in crash numbers. Overall, allowing lane splitting is potentially a component in increasing motorcycle safety, but it is just one part of this puzzle.

--------------------------------------------------------------------------------------------------*

"Notebook_structor.ipynb" is the main Jupyter Notebook file we were all working in. The "Resources" folder contains the files we used to perform our analysis. The "Output" folder is simply for one's conveinence in seeing the graphs we have created, and other files were either test files, or cache files.

------------------------------------------------------------------------------------------------

Unoriginal Code to be posted here:

  Reference for using the isin andfunction:

  selected_rows = df.loc[df['Name'].isin(names_to_select)]
  selected_rows = df.loc[~df['Name'].isin(names_to_exclude)]


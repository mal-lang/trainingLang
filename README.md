# trainingLang
A simple MAL language used to create simple models and attack graphs for machine learning agents training.

# How to compile trainingLang

1. Download and install malc: `git@github.com:mal-lang/trainingLang.git`

2. Clone this repository

3. Compile trainingLang: `malc trainingLang/src/main/mal/trainingLang.mal`

`malc` will generate a .mar-archive that can be used by MAL Toolbox to generate AttackGraphs.
TODO: Link to docs on how to do that.

# trainingLang
The goal of trainingLang is to be simple but still feature several types of assets and associations.
We want to keep number of attack steps low to result in smaller attack graphs.
exampleLang is also a simple MAL language, but too simple for any meaningful training.
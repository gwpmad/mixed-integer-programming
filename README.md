Using pyomo in a Jupyter Notebook to recreate the example here: https://brilliant.org/wiki/linear-programming/

We evolved the example slightly in order to demonstrate mixed integer programming. In the Brilliant example they use a linear example (the function would increase linearly e.g. doubling input doubles output) but in most data science problems the objective (the thing you're optimising) is non linear.

FYI integer programming is a special case of linear programming (which often doesn't have integer solutions becuase it's just lines crossing within an allowed constraint space, see the Brilliant example [here](https://ds055uzetaobb.cloudfront.net/brioche/uploads/2y7dz9w2Sj-inequality-constraints.png?width=3000)) where the solutions have to be integers. If one part of solution needs to be integer and other doesn't, that's mixed integer programming. These are both subsets of linear programming.

To set up envirnoment and run:
```
# create and activate virtual environment
python3 -m venv venv
source venv/bin/activate

# install pip in venv
pip install -U pip

# install notebook dependencies
pip install pyomo
pip install jupyter
brew install glpk

# run notebook
jupyter notebook
```

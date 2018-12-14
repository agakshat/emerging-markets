## Effect of inclusivity of political institutions and regime transitions on a nation's economy

### Work done with Alexander Bendyk

We looked at how inclusivity of political institutions of a nation affect the economic growth, and focused specifically on regime transition events, i.e. what happens to growth when a nation's political system undergoes significant changes?

The most important conclusion we reached was that it is important for positive democratic transitions to take place gradually, instead of very rapid transitions, for the economy to benefit in a meaningful way.

### Data

1. Polity IV Dataset, from the Center for Systemic Peace: [link](https://www.systemicpeace.org/polityproject.html)
2. Freedom House Data on Political Rights and Civil Liberties: [link](https://freedomhouse.org/report/freedom-world/freedom-world-2018)
3. Penn World Tables Data: [link](https://www.rug.nl/ggdc/productivity/pwt/)

### How To Use

``` bash
git clone git@github.com:agakshat/emerging-markets.git
cd emerging-markets/
virtualenv -p python3 polityenv
source $PWD/polityenv/bin/activate
python3 -m pip install --upgrade pip
pip install numpy scipy matplotlib jupyter pandas seaborn

jupyter notebook
```

This should open up a window in your browser, where you will see two notebooks: 

1. `InitDataHandling.ipynb`: Loads up data from Excel sheets and saves it in a desirable format in `.npy` format, however you don't need to run this since the `data/` folder already has those arrays saved. If, however, you want to access some other data you can change and rerun this file accordingly.
2. `PolityAnalysis.ipynb`: Has the code for most of the analysis done on regime transitions, with commented code that should be uncommented according to what cases you want to plot graphs for

### Acknowledgements

I'd like to thank Prof. Laurence Ales for being an awesome instructor for the course and encouraging us to work on good problems

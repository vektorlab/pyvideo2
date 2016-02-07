---
Category: 'EuroPython 2014'
Copyright: 'http://creativecommons.org/licenses/by/3.0/'
Language: 'English'
SourceUrl: 'http://www.youtube.com/watch?v=2oPevmFcZxI'
Speakers: [Roberto Polli]
Tags: [Tech]
ThumbnailUrl: 'http://i.ytimg.com/vi/2oPevmFcZxI/hqdefault.jpg'
Title: 'Statistics 101 for System Administrators'
date: '2014-07-22'
---
#Statistics 101 for System Administrators

## Agenda
 * A latency issue
 * Data distribution
 * 30 seconds correlation with pearsonr
 * Combinating data
 * Plotting and the power of color

## An use case 
 - Network latency issues
 - Correlate latency with other events 
    
## First statistics 
 - we created our parsing library 
 - [using various recipes](http://chimera.labs.oreilly.com/books/1230000000393/ch06.html)
 - Having the data in a dict like

        > table = {
        >   'time': [ 1,2,3, ..],
        >   'elapsed': [ 0.12, 12.43, ..],
        >   'error': [ 2, 0, ..],
        >   'size': [123,3223, ..],
        >   'peers': [2313, 2303, ..],

 - It's easy to get max, min and standard deviation

        > print [k, max(v), min(v), stats.mean(v) ] for k,v in table.items() ]

## Distribution 
 - A distribution shows event frequency 

        > from matplotlib import pyplot
        > pyplot.hist(table['elapsed'])

 - Time and Size distributions

## (Linear) Correlation 
 - What's correlation
 - What's not correlation
 - pearsonr and probability
 - catch for linear correlation

        > from scipy.stats.stats import pearsonr
        > a, b = range(0,10), range(0,20, 2)
        > c = [randint(0,10) for x in a]
        > pearsonr(a, b), pearsonr(a,c)
        > (1.0, 0.0), (0.43, 0.2)

## Combinations 
 - using itertools.combinations
 - netfishing correlation

        >from itertools import combination
        >for f1, f2 in combinations(table, 2):
        >        r, p_value = pearsonr(table[f1], table[f2])
        >        print("the correlation between %s and %s is: %s" % (f1, f2, r))
        >        print("the probability of a given distribution (see manual) is: %s" % p_value)

## Plot always 

 - pearsonr finds *only* linear correlation
 - our eyes work better :P
 - so...plot always!
 - color is the 3d dimension of a plot!

        > from pyplot import scatter, title, xlabel, ylabel, legend
        > from pyplot import savefig, close as closefig
        >
        > for f1, f2 in combinations(table, 2):
        >    scatter(table[f1], table[2], label="%s_%s" % (f1,f2))
        >    # add legend and other labels
        >    r, p = pearsonr(table[f1], table[f2])
        >    title("Correlation: %s v %s, %s" % (f1, f2, r))
        >    xlabel(f1), ylabel(f2)
        >    legend(loc='upper left') # show the legend in a suitable corner
        >    savefig(f1 + "_" + f2 + ".png")
        >    closefig()

 
## Wrap Up! 
 - do not use pearsonr to *exclude* relation between events
 - plots may serve better
 - scatter plot can show a system thruput and exclude correlation between fields A and fields B
 - continue collecting results
 


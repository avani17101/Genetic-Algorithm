# Genetic Algorithm 
Genetic Algorithm coded for optimizing weights of a ML model.
Part of Machine Data Learning course at IIIT Hyderabad.

## Implementation details
### Fitness Function used:

Over the course of the evolution of the population, we had changed out fitness functions a few times depending on where our vectors were converging to.
Some of the fitness function used were:
    
## Crossover functions:

The function breed_parents takes two parents as an argument and returns two children:

We mainly used two combination functions to mate two chromosomes.

1. Whole Arithmetic Combination
2. Uniform Combination

### Code for Whole Arithmetic Combination:

Takes the weighted mean of both the vectors and returns two children based on the parameter $\alpha$

* This was used in the beginning since we didn't know how rough the surface was.
* This was useful in the beginning to converge fastly but this approach gets saturated quite soon because the system seems to be very spikey so we had to change our approach.

### Code for Uniform Combination:
   
* Randomly switches genes of two chromosomes and returns 2 new chromosomes.
* Particulary useful in systems where even small changes in parameters lead to a lot of change in accuracy.
   
## Mutation function:

For mutation, we have two parameters mutation_probabilty and mutation_magnitude.

**mutation_prob** : How many genes in the chromosome will be altered.

**mutation_mag** : How large would the magnitude of mutation be.


## Contributors
* Bhuvanesh Sridharan
* Avani Gupta

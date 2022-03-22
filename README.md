# Six-Degrees-of-Kevin-Bacon
### Computing the degrees of separation between Kevin Bacon and other movie actors

"Six Degrees of Kevin Bacon or 'Bacon's Law' is a game based on the 'six degrees of separation' concept, which posits that any two people on Earth are six or fewer acquaintance links apart. Movie buffs challenge each other to find the shortest path between an arbitrary actor and prolific actor Kevin Bacon. It rests on the assumption that anyone involved in the Hollywood film industry can be linked through their film roles to Bacon within six steps." (via wikipedia)

In this project, we build a large graph of movies and stars and compute the degrees of separation between Kevin Bacon and other performers.

We have our data in "movies.text" file. Each line of this file starts with a movie name followed by a "/"-delimited list of those appearing in the movie (notice that the names are listed as last, first).

For example, a partial listing of the movie Fight Club is:
> Fight Club (1999)/Termo, Leonard/Arquette, Richmond/Rosario, Marcio (I)/Pontino, J.T./Peddy, ...

We parse this file to create a graph of all of the movies and performers. We represent the graph using a dictionary indexed on the performer's name (a string).

After building the graph, we use breadth-first search to determine the shortest path between two performers.

**Language:** All code is in Python. I used Jupyter Notebook as development environment

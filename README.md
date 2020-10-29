# Deduplication Research, Summer 2020, Andy Kim

## Inspirations and Background Research
This repository is the culmination of my research on entity resolution - the task of merging records in a real-life database, often using machine learning. As it is with many machine learning applications, there have been many advances in the field, such as using relational data [(Bhattacharya, Getoor)](https://www.norc.org/pdfs/may%202011%20personal%20validation%20and%20entity%20resolution%20conference/collective%20entity%20resolution%20in%20relational%20data_pverconf_may2011.pdf) and active learning, as discussed in [Mikhail Bilenko’s PhD dissertation](https://www.cs.utexas.edu/~ml/papers/marlin-dissertation-06.pdf). [Dedupe](https://github.com/dedupeio/dedupe), the tool I utilized for this project, is based on this dissertation.
To gain a better understanding of entity resolution and active learning, I explored multiple lectures, like [this talk](https://www.youtube.com/watch?v=_Ql5vfOPxZU) from ICML 2019, and [this talk]( https://www.youtube.com/watch?v=2Drw9plALIM) given at Microsoft by Professor Héctor García-Molina of Stanford University.

## What is the data?
The `Illinois-example` project is an improved and streamlined version of this [repository](https://github.com/dedupeio/dedupe-examples/tree/master/pgsql_big_dedupe_example), while the `whitehouse` project is the code adapted for an entirely new dataset – the White House Visitors Log from parts of 2011, accessible [here](https://obamawhitehouse.archives.gov/briefing-room/disclosures/visitor-records).

## How do I run this?

Set up a new conda environment with the `.yml` file, and set up a local Postgres DB. Make sure to run the `.ipynb` files suffixed with '-data' first, as those are needed to preprocess the data. All data is included in the repository.

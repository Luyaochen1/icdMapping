# icd2pheotype - The fastest way to identify phenotypes from icd (9 or 10) list !

With preloaded phenotype repositories, use this package to identify phenotype(s) from a list of ICD 9/10   

#Overview


## Usage


###  Getting it

To download icd2pheotype , either clone this github repo or simply use Pypi via pip.
```sh
$ pip install icd2pheotype
```

### Using it

First, import icd2pheotype package

```Python
import icd2pheotype
```

And you are ready to go!  

## Functions
printrepos() - return all the repositories in the packages
getrepo( reponame)  - returen a repositories by name
printphenotypes( reponame )  - return phenotypes defined in the repository 
icd2phenotype(icdlist,reponame) - map icd list to phenotypes
 
 ## Examples



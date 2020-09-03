# icdMapping - The fastest way to identify diseases from icd (9 or 10) list !

With preloaded diseases repositories, use this package to identify disease(s) from a list of ICD 9/10   

#Overview


## Usage


###  Getting it

To download icdMapping , either clone this github repo or simply use Pypi via pip.

```sh
$ pip install icdMapping
```

### Using it

First, import icdMapping package

```Python
import icdMapping
```

And you are ready to go!  

## Functions
printrepos() - return all the repositories in the packages
getrepo( reponame)  - returen a repositories by name
printdiseases( reponame )  - return diseases defined in the repository 
icdMapping(icdlist,reponame) - map icd list to diseases
 
 ## Examples

```Python
import icdMapping as ip
import pandas as pd
```
```Python
ip.printrepos()
```
['icd10_map_names_ccs', 'icd9cm_hierarchy', 'icd9_map_multi_ccs', 'icd10_sub_chapters', 'icd10_map_quan_deyo', 'icd10cm2019', 'icd10_map_ahrq', 'icd9_map_cc', 'icd9_names_single_ccs', 'icd10_map_pccc_dx', 'icd9_map_quan_elix', 'icd9_majors', 'icd10_map_elix', 'icd9cm2014_leaf', 'icd9_map_pccc_dx', 'icd9_map_charlson', 'icd10_map_quan_elix', 'vermont_dx', 'icd_map_cc_hcc', 'icd10_map_ccs', 'uranium_pathology', 'icd10_map_charlson', 'icd10_map_pccc_pcs', 'icd9_map_ahrq', 'icd9_map_quan_deyo', 'icd9_map_single_ccs', 'icd9_map_elix', 'icd10_map_ahrq_pcs', 'icd9_names_multi_ccs', 'icd9_map_pccc_pcs', 'icd10_map_cc']

```Python
 ip.printdiseases('icd9_map_pccc_dx');
```
['hemato_immu', 'gi', 'transplant', 'respiratory', 'congeni_genetic', 'renal', 'neonatal', 'malignancy', 'tech_dep', 'cvd', 'neuromusc', 'metabolic']

```Python
test_icds = ['39891', '40201', '40211', '40291', '40401', '40403', '40411', '40413', '40491', '40493', '428', '4280', '42800', '42801', '42802']
print(ip.icd2diseases(test_icds,'icd9_map_ahrq'))
```
![result](https://github.com/Luyaochen1/icdMapping/blob/master/pics/icd2phenotype_result.JPG)
 

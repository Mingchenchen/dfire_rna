

# DFIRE-RNA

Knowledge-based statistical energy based on DFIRE reference state.

# Install

## Linux

Use cmake

```
mkdir build
cd build
cmake ..
make
```


or use make

```
# This bash script writes DFIRE_RNA_HOME to the .bashrc and calls make
# re-open terminal to get .bashrc sourced
./install.sh
```

# Usage

```
# run dfire_rna witout parameters

#######################################################
# Calculate dfire_rna score for a pdb or a list of pdbs
#######################################################
Usage: ./bin/dfire_rna pdb 
   or: ./bin/dfire_rna [ options ] 
Options:
   pdb [ pdb2 pdb3 ...], input RNA structures in pdb format
   -d directory,         OPTIONAL, override default directory of energyfiles
                         default: dfire_rna/data/energyfiles
   -norm                 normalize DFIRE score by RNA length (experimental)
   -l pdblist,           A list of absolute paths to pdb files (plain text) UTF-8 encoding

```


# Example

```
cd example
dfire_rna *.pdb

# output:
#
# 1a9nR.pdb -10956.515269  
# 3b58ABC.pdb -45025.865086  
# 5e3hBC.pdb -17838.716027  
```

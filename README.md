# machine-translator
A Phrase-Based Machine-Translation System

__Presentation Link__ : https://bit.ly/2IRlluf

## Quickstart
### Requirements
- Python 2 and Python 3 
- GIZA++
- IRSTLM
- Stanford Parser
- cfilt_preorder
- NLTK 3.4.1

Currently, only Linux systems are supported.

### Installation
#### Linux/Unix
```$ git clone https://github.com/Axle7XStriker/machine-translator.git```  
```$ cd machine-translator```

### Usage
The package already contains all the files pre-installed in the ```src``` directory, you just need to copy cfilt_preorder and Stanford Parser in the ```src/utils``` directory. The package can be accessed using the ```src/build.sh``` executable:
```
$ cd src
$ ./build.sh help

Usage: ./build.sh COMMAND

Commands:
clean         Removes all the generated files
generate      Generate the training, testing and their word aligned files from the parallel corpus
train         Train the Phrase-Based Statistical Machine Translation model
test          Run the model on the testset and Evaluate the translations generated by the model
build         Build the whole PBSMT model by performing clean, generate and train together
help          Display help menu
```
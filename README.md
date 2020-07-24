
# cpplint-example
This is cpplint example


(1) To lint on specific file 

$ cpplint example.cpp

(2) To get list of all cpplint filters 

$ cpplint --filter=

(3) To Suppess a kind of filter , create file CPPLINT.cfg , add filters you want to supress 
in file like , filter=-legal/copyright,-build/namespaces

$ cat CPPLINT.cfg

filter=-legal/copyright,-build/namespaces

(4) To lint a folder and exlude some paths , you can use

$ cpplint --exclude build --exclude test-utils/ --recursive .

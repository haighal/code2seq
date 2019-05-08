### Notes on Modifications to Code2seq (Alon et al, ICLR '19)
Alex Haigh
Snap Group, May 2019

##### 5/7/19

General plan of attack:
- Run their pretrained model on java-large (preprocessed) to verify results
- Retrain their model from scratch on the pre-parsed dataset
- Parse the dataset myself and repeat
- Build a pipeline for python (look @Code2vec to see they have a python pipeline) and see if we can recover the whole Java AST for use with Michele/Dylan's masked transformer

- How do they do MethodNaming in code2vec?

virtualenv -p /usr/bin/python3.5 env
pip install --upgrade pip
pip install --upgrade tensorflow-gpu
pip install requests
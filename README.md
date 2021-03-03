# ProSOUL

ProSOUL (**P**ropaganda **S**potting in **O**nline **U**rdu **L**anguage) framework to identify propaganda content in the Urdu language.


# Dataset
The corpus is developed by translating English QCRI’s propaganda (Qprop) dataset. The English dataset was downloaded from Zenodo and translated using Google translate. Our corpus contains 11,574 news articles labelled as propaganda or non-propaganda. 
## Data Format
Two text files are provided, one for propaganda and other for non-propaganda. Every line in the text file represents an article. The data is tab-separated and contains three fields:

* Article text
* Article source
* Article date

# Urdu LIWC
The LIWC dictionary is build by translating the English LIWC dictionary using the Google translate service. The file _LIWC_URDU.dic_ contains the data in the standard format of LIWC dictionay. 
To use the Urdu LIWC dictionary python, follwoing steps can be followed:


* Intall the LIWC library using pip with the command _pip install liwc_
* Import and read the dicitonary using following code.
`import liwc
parse, category_names = liwc.load_token_parser('LIWC_URDU.dic')
` 
* _parse_ will contain the words and the categories assigned to these words will be stored in _category_names_. 
# Credits

`@article{prosoul,
 title={ProSOUL: A Framework to IdentifyPropaganda from Online Urdu Content},
 author={Kausar, Soufia and Tahir, Bilal and Mehmood, Muhammad Amir},
 journal={IEEE Access},
 volume={},
 pages={},
 year={2020},
 publisher={IEEE}
}`

# Authors
* Soufia Kausar
* Bilal Tahir
* Muhammad Amir Mehmood



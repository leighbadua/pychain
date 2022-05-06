# Pychain Ledger
This prototype demonstrates the usage of blockchain-based ledger system. It is complimented with the a user-friendly web interface through the use of Streamlit. This ledger would allow partner banks to conduct financial transactions (to transfer money between sends and receivers) and to verify the integrity of the data in the ledger. 

### Technologies
This project uses the following libraries and dependencies:
+ [**Anaconda**](https://docs.anaconda.com/): an open source package and environment management system.
+ [**Pandas**](https://pandas.pydata.org/docs/getting_started/index.html): (included in Anaconda) a Python package data analysis toolkit.
+ [**Python**](https://www.python.org/): is a programming language that offers a vast modules and libraries such as dataclass, typing, hashlib, datetime, and much more.
+ [**Streamlit**](https://docs.streamlit.io/library/get-started): a Python library that works only with Python files (.py files). It quickly turns Python scripts into shareable web apps. For this application we will create a user-friendly webpage interface for a blockchain. 


## Installation Guide

Activate your working environment and run the following command in your terminal:

```
pip install streamlit
```

## Usage 
Option 1:
1. Click on the link to directly use the Streamlit web interface https://share.streamlit.io/leighbadua/pychain/main/pychain.py

    **OR**

2. Activate your local working environment
3. Clone the repository `https://github.com/leighbadua/pychain.git`
4. From the repo launch `pychain.py` by typing the following into the terminal, `streamlit run pychain.py`

    ![image](https://user-images.githubusercontent.com/96001018/167096108-b1ba6f19-1f14-4024-ab71-8cc021af6766.png)

### Features

The image shows the Streamlit application in use. The user is required to enter text in the 'Sender' and 'Receiver' lines and include an amount value into the 'Amount' line. It will be stored in the record dataclass. 
Once these fields are filled out, the user can click `Add Block` button to add the block data container to the Pychain Ledger. 


![pychain_1](https://user-images.githubusercontent.com/96001018/167097783-865b045d-d7e3-4170-b2d6-ae0e3cadea3d.jpg)

### Streamlit Sidebar
***Block Difficulty*** slider widget - Allows the user to change the blockchain's difficulty level. 

***Block Inspector*** dropdown bar - Displays details to each Block transaction. 

<img width="186" alt="image" src="https://user-images.githubusercontent.com/96001018/167212038-d545e31d-6f2a-4298-99c5-07b67c4b9caf.png">

![image](https://user-images.githubusercontent.com/96001018/167212117-8690aea4-af74-4a14-9ae9-80f1eb79430a.png)

### Pychain Ledger

***Record*** Shows the user's input text that is store in this column per transaction. 

***creator_id, timestamp*** Provides information about who created the block and when. These are attributes to the record data class. 

***prev_hash*** An attribute that stores the hash of the last block.

***nonce*** Random number issued for authentication protocol. 

The `Validate Chain` button will run the proof_of_work method that accepts a block and gets the block updated. This algorithm will check whether the hash meets the system requirements.

![pychain_ledger_validated](https://user-images.githubusercontent.com/96001018/167097797-1a8b4ff0-ade1-4a11-993d-6328692460f3.jpg)


Display in terminal after selecting the `Validate Chain` button.

   ![image](https://user-images.githubusercontent.com/96001018/167098696-ddbcffef-3d40-41e9-a8ec-cc9e74a6e8d3.png)


## Contributors

Leigh Anne Badua leighbadua@gmail.com 


## License

MIT

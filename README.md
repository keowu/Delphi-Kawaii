# Delphi-Kawaii

Delphi-Kawaii is a plugin for Ida Pro to perform the parsing of the MAP file (generated by the IDR) and in this way rescue all the Delphi symbols. I decided to create the parser for the MAP file because performing reverse engineering is much better in Ida than in IDR.


## Install

Installation is extremely simple, considering that the plugin does not use any other lib that is not from Ida. You just need to download the Delphi-Kawaii.py file and place it inside Ida's plugins folder. If you want to choose a hotkey for the plugin you can edit the file on line 50
```python
    wanted_hotkey = ""
```
## Usage

To use the plugin you will need to analyze the delphi binary inside the IDR and after that create the MAP file of the analyzed binary.

&nbsp;
![App Screenshot](https://github.com/Xienim/Delphi-Kawaii/blob/main/IDR.png)

After getting the MAP file from your delphi file, you will load your delphi binary in Ida and start the plugin. It will ask for the full PATH of your MAP file and after that it will import all symbols into idb. It is much easier to analyze the binary within Ida and with the symbols generated by IDR.

## Demo

### Functions before import

&nbsp;
![App Screenshot](https://github.com/Xienim/Delphi-Kawaii/blob/main/Func_Before.png)

&nbsp;
![App Screenshot](https://github.com/Xienim/Delphi-Kawaii/blob/main/Dis_Before.png)

### Functions after import

&nbsp;
![App Screenshot](https://github.com/Xienim/Delphi-Kawaii/blob/main/Func_After.png)

&nbsp;
![App Screenshot](https://github.com/Xienim/Delphi-Kawaii/blob/main/Dis_After.png)

## To do
- import the IDR engine to resolve symbols directly in the plugin.

## Credits

IDR is an OpenSource project and it did most of the process of resolving the Delphi symbols. Link to the project -> https://github.com/crypto2011/IDR

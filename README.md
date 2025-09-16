# python-automation
script python for renaming many files in a folder
#programa que automatiza a renomeiação de vários arquivos em uma pasta

import os


#variavel para armazenar o caminho da pasta a ser escolhida 
folder = r'C:\pasta\\'


#percorrer todos os arquivos dentro da pasta escolhida 
for file_name in os.list_dir(folder):
    old_name = folder + file_name
    new_name = folder + 'AAAA -'+ file_name
    os.rename(old_name, new_name) 

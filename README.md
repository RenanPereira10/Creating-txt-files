# Creating-txt-files
import os
path = r'C:\\Users\\-\\Documents\\Desafio'
os.makedirs(path, exist_ok=True)
with open('C:\\Users\\-\\Desktop\\Python.txt') as file:
    for country in file:
        country = country.strip()
        with open(f'{path}/{country}.txt', 'w') as saida:
            saida.write(country)

##solution 5##
a. ([A-Z][a-z\d]+)(?=([A-Z][a-z\d]+))

b. [\w\s] gets rid of all characters,numbers and whitespace, leaving only special characters.

c. [^\\|\{\}":?<>,.\;'\[\]=/-/!@#$%^&*\(\)_\-\+`~] This leaves only special characters. 

d. ^-?\d*[0|2|4|6|8]{1,2}$

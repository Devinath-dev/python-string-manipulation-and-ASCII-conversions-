# python-string-manipulation-and-ASCII-conversions-
# # 7. convert capital letters into small letters and smalls to capitals.

# Approach-01
h = 'PyThOn'
b = ''
for i in h:
    if i.islower():
        b += i.upper()
    elif i.isupper():
        b += i.lower()
    else:
        b += i
print(b)

# Approach-02
j = 'PyThOn'
b = ''

for x in j:
    if ord(x) >= 65 and ord(x) <= 90:   
        b += chr(ord(x) + 32)          
    elif ord(x) >= 97 and ord(x) <= 122: 
        b += chr(ord(x) - 32)          

print(b)

[![Open in Codespaces](https://classroom.github.com/assets/launch-codespace-f4981d0f882b2a3f0472912d15f9806d57e124e0fc890972558857b51b24a6f9.svg)](https://classroom.github.com/open-in-codespaces?assignment_repo_id=10512543)
<!--
[Link to Chap 5 Lab18](https://docs.google.com/presentation/d/1r3h2R9JwK9HK_U2Ia-zncL0BSjHV6Giu6ugNJ6yZpgc/edit#slide=id.g1715447b552_0_27)

![Lab 16](https://nimbus-screenshots.s3.amazonaws.com/s/e634571b38c8923031df60fc7fc2fe3f.png)
-->

## Complete the "main.py"
email = input('Enter your string ')

flag = True
if not email[0].isalpha():
    flag = False
lenemail = len(email)
if lenemail <= 5 or lenemail >= 30:
    flag = False
if email.find('@') == -1:
    flag = False
else:
    atidx = email.find('@')
if email[atidx+1:].find('.') == -1:
    flag = False

print (flag)

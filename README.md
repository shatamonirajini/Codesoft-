import string
import random

s1=string.ascii_lowercase
s2= string.ascii_uppercase
s3=string.digits
s4=string.punctuation

print("********welcome to password generator********")

password=int(input("enter the length of the password:\n"))


s1=int(input("enter the  no.of ascii_lowercase in your password:\n "))

lowercase=input("enter the choose of ascii_lowercase in yor password:\n")

s2=int(input("enter the  no.of ascii_uppercase in your password:\n "))

uppercase=input("enter the choose of ascii_uppercase in yor password:\n")

s3=int(input("enter the  no.of digits in your password:\n "))

digits=input("enter the choose of digits in yor password:\n")

s4=int(input("enter the  no.of punctuation in your password:\n "))

punctuation=input("enter the choose of punctuation in yor password:\n")


created_password =[]
created_password.extend(list(lowercase))
created_password.extend(list(uppercase))
created_password.extend(list(digits))
created_password.extend(list(punctuation))

random.shuffle(created_password)

print("".join(created_password[0:password]))


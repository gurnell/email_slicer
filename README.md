## Email_slicer
### Beginner python project
This project is a simple email slicer created with **Python v3.9.7** with **Juypter Notebook**. 

The slicer takes an email address as input and slices it to produce username and associated domain.

 ## About

 ##### We begin by asking the user to input their email.

 ```python

email = input("Enter Your Email: ").strip()  

```

In the above code snippet, we use **input()** method to get input from the user, then save it to the **email** variable.

The **strip()** method removes unwanted and additional spaces on both sides of the strings. This will ensure that we only get the email from the user. 

##### The next step

```python

username = email[:email.index('@')]
domain = email[email.index('@') + 1:]

```

The code above separates the username with the domain. The variable **username** selects the part of the string that comes
before the **@** as the username. **index()** returns the position at the first occurrence of the specified value which in this case is @.
We are also using the slicing operator **(:)** . The **domain** variable also works the same.

Let us take for example an email like **guowili16@gmail.com**. The index() function will interpret the email as email[:9], because the @ is
found at index **9**. So the part of the string that comes before index 9 will be taken and the rest of the string will be ignored. The vice versa
is true for the part of the string that comes after @ when picking the domain name.

##### Finally we print the output

```python

print(f"Your username is {username} & domain is {domain}")  

```

We use the f_string to allow us to directly place our variables in the output string. The f-string is very useful as it has minimal syntax for 
string formatting.

The project is for beginners. If you are a beginner like me, this is a good way to practice Python.
















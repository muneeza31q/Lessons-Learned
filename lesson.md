6/07/2022

Lesson 1: Python Dictionary Using If-else Statement


This post will discuss the use of an if-else statement for a dictionary in Python.

Before we dive in, we should discuss what is a dictionary. A dictionary is a set where it stores a mapping between a set of keys and a set of values. Keys are immutable (not changeable) items. Values are mutable (changeable) items. An example is shown here:

```python
import random
import sys
capital_dict={
    'Colorado': 'Denver',
    'Hawaii': 'Honolulu',
    'California': 'Sacramento',
    'Louisiana': 'Baton Rouge',
    'New York': 'Albany',
    'Tennessee': 'Nashville',
    'Texas': 'Austin',
    'Utah': 'Salt Lake City',
    'Alaska': 'Juneau',
    'Wyoming': 'Cheyenne'  
}
# key is the state and value is the capital
```

Now that we have our dictionary created, we will create a program that will print the state capitals of those states when the user enters a state name. This is where using the if-else statement will be used.

```python
States=list(capital_dict.keys())
capitals=list(capital_dict.values())
print ('Hello!')
state=random.choice(States) # randomly select 10 states
capital= capital_dict[state]
user_guess = input('Enter the state %s - ' %state)
if user_guess.title() == state:
        print('The capital is %s.' %capital)
else:
        print('That state is not in our database')
```

Let’s use the example above.

Here, the list of the keys from the capital_dict will be defined as “States”. For “state”, “States” should be randomly picked. Make sure to import random at the beginning of your code. For “capital”, this will pull the “state” from capital_dict. Moving to user_guess, this defines the input statement that will be shown on the screen. In this case, the statement ‘The capital is %s.’ The % represents a wildcard for the state. Now, we can jump to the if-else statement. Here, if the user_guess is any state from the list, for example California, the input will look like this:

<div id="badges">
<a href="https://miro.medium.com/max/1750/1*dZfKN4q53dotm30YHo4png.png">
  <img src="https://miro.medium.com/max/1750/1*dZfKN4q53dotm30YHo4png.png"/>
  </a>
  </div>


In the blank space, we would type California as California is stated on the left side. Once we press the Enter button, its capital will show.

<div id="badges">
<a href="https://miro.medium.com/max/1750/1*THBmpGADGw6SYnjFn4-E_g.png">
  <img src="https://miro.medium.com/max/1750/1*THBmpGADGw6SYnjFn4-E_g.png"/>
  </a>
  </div>

As for the else statement, the statement serves as a false statement if entering a different state or capital that is not mentioned from the capital_dict list. The output is shown below:

<div id="badges">
<a href="https://miro.medium.com/max/1750/1*m_ZWqpK4WBvrT6c1rp5fRQ.png">
  <img src="https://miro.medium.com/max/1750/1*m_ZWqpK4WBvrT6c1rp5fRQ.png"/>
  </a>
  </div>

Thank you for reading this post! I hope you learned a tip from this post. Feel free to provide feedback anytime.

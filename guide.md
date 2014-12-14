Github link to what they are building - version
Programming Fundamentals in Python - 2 hours
Introduction
What is Python?
Python is a scripting programming language known for both its simplicity and wide breadth of applications. For this reason it is considered one of the best languages for beginners. Used for everything from Web Development to Scientific Computing, Python is referred to as a “general purpose” language by the greater programming community.

Many Python programmers (aka “Pythonistas”) love this language because it maintains a certain philosophy of best practices, described in Tim Peter’s famous “Zen of Python.” There is a large Python community both off and online that is welcoming and supportive of beginners, and you can find a plethora of additional materials in the resources section of this guide.

About this Guide:
This guide will follow Thinkful’s project-driven learning philosophy, i.e. the best way to learn something is to build a project. You will be creating a “Pypet” (“Python-pet”) of your choosing. As you learn new Python concepts you will be able to add new features to your Pypet. This way you will be able to put your new knowledge to use right away and actually create a project in Python.

This guide will assume no programming knowledge. It will also go beyond teaching you basic Python concepts and show you how to actually run Python files on your computer. The best way to use1 this guide is to go in order. After this guide you will feel comfortable using strings, etc etc and have a Pypet that you can interact with and show off!


Choose your Pypet:
Go ahead and choose a Pypet now so that we can begin! Feel free to customize your Pypet, but here are a few options. Try to keep you Pypet height limited to just one line for now as it will make the initial steps easier to follow.

Pycat


(=^o.o^=)__
Pymouse


<:3 )~~~~
Py? (you choose!)


(^‘*m*’^)

Input box to tweet out Pypet??

Setup

Nitrous.IO
The first stage of our journey will be setting up a development environment which you can work in – your Nitrous.IO box. Nitrous.io is the faster way to get your Python development environment up and running.
Nitrous.io is a service which gives you web based access to a configurable development environment. The environment is run on a remote linux box which has Ubuntu Linux preinstalled. The free version of Nitrous.io, which you'll be using in this course, gives you a single box, but you can develop multiple apps from this box. When you log in to a Nitrous.io box, you get access to command line console windows and a built in text editor, amongst other tools. 
Setting up Nitrous.IO
Create a Nitrous.io Account: First you’ll need to head over to Nitrous.IO to create a new account. After you submit your username, email, and password, you’ll need to wait a minute or two for a confirmation email from Nitrous.IO. Click through on the activation link in the confirmation email, and you’ll be taken to a dialog for creating a new box.
Create a Box: In the Create Your First Box dialogue, choose the Python/Django option. You can go with the default name for your box, or set it to a name of your own choosing. Select the region you want your box to be served from (for this course, probably the region you reside in). Then click Create Box. You’ll have to wait while your box is provisioned. Once that’s complete you should click the IDE button to be taken to it.
Take a Tour of Your Box: Great! You’ve now got a powerful, cloud-based development environment that comes pre-installed with Python! Let's take a quick tour:
In the left-most panel, you’ll see the File Browser. Here you can navigate the files in your home folder. At this point, you will just have the "workspace" folder and a README file introducing you to Nitrous.IO. When you have more files, you can open them in Nitrous.IO’s text editor by double clicking on them in the File Broswer.
The middle panel is the Text Editor. This is where you can write and edit code.
The right panel is for chatting if you’re using Nitrous.io in collaborative mode. If you’re flying solo, you should close this window by clicking the X in the upper right hand corner so you get more screen real estate.
The bottom panel is for your consoles. By default, one console will be open when you visit your box, but you can open additional consoles by clicking the plus button. Note that you can also resize your console by dragging the bar the console tabs appear in. If you’d like to maximize the console window, you can do this by clicking the icon in the top right corner of the console window.
 Console Commands
Do not be alarmed! We are going to break down the Terminal and make it super simple. In order to be a successful Pythonista you should learn basic Terminal commands. 

You will access your console from your nitrous. There are only 6 commands you need to learn in order to successfully run Python files!
Technical jargon alert: “directory” is just a fancy programmer way of saying folder!
pwd - print working directory
Type “pwd” into your terminal and hit enter. This tells you which directory (aka folder) you are currently in. This is very similar to using Mac’s Finder or Windows’ X except it’s the cool programmer version.
ls - list
Type “ls” into your terminal and press enter. This will list all the files and folders that are in your current directory.
cd - change directory
Type “cd filename” and press enter in order to move into a file. You can only use “cd” on files inside the folder you are currently in.
If you want to go up one folder type “cd ..” and press enter.
Typing “cd” alone will return you to your home directory
Play around and try moving through some files!
python your_python_file.py
In order to run a Python file you will have use the following format: “python file_name.py”. 

Go impress your friends with your new AMAZING Terminal skills (and then continue on so you can print out your Pypet using Python!)
	
Running Python for the first time!
Open your “pypet.py” file in Nitrous and let’s add a welcome message for your Pypet program using a print statement.

print 'Welome to Pypet!'

Save your file!
Go back to your Terminal and make sure you “cd” into the directory that contains your pypet.py file. Now type “python pypet.py” and see what happens!

Call to Action - Stuck? We want to help, tweet at us

Creating your Pypet

The Pypet you will create is going to have certain attributes. For example we need to give it a name. Below we have set a variable called name equal to 'Mr Fluffy'.  In programming variables simply store data for us, but there are a variety of different types of data.

name = 'Mr Fluffy'

In this case, name is something called a string because 'Mr Fluffy' has quotations around it. A string is just a set of characters surrounded by quotations. Variables on the other hand do not have quotations. Let’s look at some additional data types.

weight = 9.5
hungry = False

A Boolean stores a value of either True or False. A float is a number that can have decimals. An integer is a whole number. Now for fun we will include another variable that is a string containing “photo” of our pet!

name = 'Mr Fluffy'
hungry = False
weight = 9.5
toys = 5
photo = '(=^o.o^=)__'

We need a way to tell Python that all of these variables represent one cat. One way for us to do this is to use a Python dictionary. Dictionaries are a way of storing multiple variables that have different values.

cat = {}
cat['name'] = 'Mr Fluffy'
cat['hungry'] = True
cat['weight'] = 9.5
cat['toys'] = 5
cat['photo'] = '(=^o.o^=)__'

Here we’ve created an empty dictionary called cat = {}. Then on each sequential line we add new cat attributes! Let’s go ahead and add a print statement to see our first pypet! By now your code should look like this except you should feel free to customize away.

print 'Welome to Pypet!'

cat = {}
cat['name'] = 'Mr Fluffy'
cat['hungry'] = True
cat['weight'] = 9.5
cat['toys'] = 5
cat['photo'] = '(=^o.o^=)__'

print cat

Call to Action - tweet a screenshot of your pypet @Thinkful so we can share your creation with the world!

Feeding your Pypet - Functions and If Statements

Now we are going learn how to “feed” your pypet using a Python function. A function is a block of organized, reusable code that is used to perform a single, related action. First we must define our function before we actually use it. This particular feed()function changes our pypet’s “hungry” attribute to False to show that it is no longer hungry.

def feed(cat):
		cat['hungry'] = False

You can pass variables into functions (such as we did with cat above). If you plan on using a variable inside of your function you must first pass in into the function. Since we have passed cat into the function we can now change cat['hungry'] = False. 

We should also increase the Pypet’s weight a bit since it has eaten. Floats and integers can be increased by using the following notation.

def feed(cat):
		cat['hungry'] = False
		cat['weight']+=1

Try setting your original pypet’s variable to True and then call the function by writting feed(cat) at the bottom like so:

print 'Welome to Pypet!'

cat = {}
cat['name'] = 'Mr Fluffy'
cat['hungry'] = True
cat['weight'] = 9.5
cat['photo'] = '(=^o.o^=)__'

print cat

def feed(cat):
		cat['hungry'] = False
		cat['weight']+=1

feed(cat)

print cat #The Pypet will now weigh more now that he has eaten

When the cat is printed out the second time his weight attribute will have increased. But what if our pypet is now hungry? We need to take into account whether or not the hungry variable is set to True or False.

In order to know whether our Pypet is hungry, we are going to set a condition called an if statement. If the Pypet is hungry the program will set his hungry variable to False and increase his weight. If the Pypet is not hungry then nothing will happen.

def feed(cat):
	if cat['hungry']:
		cat['hungry'] = False
		cat['weight']+=1
	else:

print cat
feed(cat)
print cat

YOU CAN ADD THE CONCATENATE BIT IF YOU HAVE ROOM.


Friends for your Pypet! - For Loops and Lists

Let’s create another Pypet!

mouse = {}
mouse['name'] = 'Mouse'
mouse['photo'] = '<:3 )~~~~'
mouse['hungry'] = False
mouse['weight'] = 1.5

Now that we have more than one Pypet we can store them in a Python list. A list is another data type; list stores variables in order like so:

pets = [cat, mouse]

An easy way for us to access the variables in this list is to use something in Python called a for loop. The for loop in Python has the ability to iterate over the items of any sequence, such as a list or a string.

for pet in pets:
	print pet

Call to Action - tweet a picture of your pypet @Thinkful so we can share your creation with the world

Conclusion & Resources

This guide just shows you the beginning of what you can do with Python. If you enjoyed the work you’ve done here, go through any of the additional resources below. If you are stuck feel free to tweet @Thinkful and we would love to help you. Also definitely tweet us a picture of your Pypet code! Feel free to customize any or all of your project and try new things. We have placed a final version of our Pypet on github if you would like to take a look at the code! Perhaps you want to keep track of health points or create a play() function?

http://learnpythonthehardway.org/




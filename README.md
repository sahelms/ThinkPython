# ThinkPython
Exercises in ThinkPython 2





# Think Python 2, Exercise 3.1

def rightJustify (word):
    spacesNum = 70-len(word)
    print((' '*spacesNum)+word)

rightJustify ('Monty')


# Exercise 3.2

def printSpam ():
    print ('Spam')
    
def doTwice (f,ar):
    f (ar)
    f (ar)
    
def printTwice(bruce):
    print(bruce)
    print(bruce)
    
# doTwice (printTwice,'Spam')

def doFour (f1,ar):
    doTwice (f1,ar)
    doTwice (f1,ar)
    
doFour (printTwice,'Spam')

# Exercise 3.3
1. 
def printTable (rows, columns, size):
    horizontal = ((('+'+((('-'*size)+'+')*columns)))+"\n")
    vertical = ((('|'+(((' '*size)+'|')*columns)))+"\n")
    group = ((vertical*size)+horizontal)
    table = (horizontal+(group*rows))
    print (table)

printTable (2,2,4)

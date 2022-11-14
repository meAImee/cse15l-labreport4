# LabReport4 - Aimee He
# Part 1: Editing from the command line: vim
> I am choosing the following task: \
Changing the name of the **start** parameter and its uses to **base**.

## Preparation:
1. Clone the repository by typing the folling in terminal:
```
$ git clone https://github.com/ucsd-cse15l-f22/skill-demo1 week6-skill-demo1 
```
2. Enter **vim** for **DocSearchServer.java**:
```
$ vim DocSearchServer.java
```


## Shortest Squence of **vim** Commands(17 keys in total):
```
:%s/start/base/g<Enter>
```

* the `:%s` command means search and replace in the whole file
* `start` means search `start` in the whole document
* `base` means replace the all `start` to `base`
* `g` means "global substitution"

After typing in the commands, the file **DocSearchServer.java** should look like this:



# Part 2: The Two Options of Editing

## Option 1: 

### Start in VSCode and make the edit there, then scp the file to the remote server and run it there to confirm it works

**Time Taken**: 61 seconds

## Option 2:
### Start already logged into a ssh session. Then, make the edit for the task you chose in Vim, then exit Vim and run bash test.sh

**Time Taken**: 63 seconds

## Question 1:
### Which of these two styles would you prefer using if you had to work on a program that you were running remotely, and why?

**Answer 1:** I would prefer using the first method(editing offline and then scpit to the server). I prefer this option because I am more used to work locally. Setting files well before **scp**ing it to remoter server would make me feel things more in control.

## Question 2:
### What about the project or task might factor into your decision one way or another? (If nothing would affect your decision, say so and why!)

**Answer 2:** If there's multiple files in one project I have to edit at the same time, I would prefer using the second option because of two reasons:
* I would not have to do scp multiple times.
* It will garantee that I am not messing up with project structure when their is mutiple folders in different folders.
* It is likely I wouldn't be able to finish the task once if there's multiple edits needed. Therefore working remotely would give me access to the latest version of edited documents anywhere anytime. (While for option 1, to edit remotely, I have to scp everytime after each time I make some changes.)


---
title: You already know how to code - Part Two
date: 2022-07-05
---

In part one, we learned that you already know how to code and probably do it every day.
You only need to learn the syntax of the programming language you choose to code in.

This time, we will do some actual coding to bring your inner coder out.

First we will need a place write and run the code, so open <a href="https://replit.com/languages/python3" target="_blank">ReplIt</a> on a new tab to follow along.
At the end of this article, you will have enough essential coding skill to progress on your own.

I request you follow along, do not copy-paste the code; read and type everything yourself. 

> Repetition is how we learn.  
> Repetition is how we learn.  
> Repetition is how we learn.  
> Repetition is….  

I hope you got the notion.

Our main objective is to learn to start thinking like a programmer. To achieve our goal, we will try to visualize how the tiny features of your phone work.

So go ahead and create three new contacts but with actual code this time:

```
akash = 9999999999
abc = 8888888888
xyz = 7777777777
```

Now we will try to write the code to send a message to one of the saved contacts via WhatsApp.
Sending a message is the primary `function` of WhatsApp. We send different messages to different contacts daily. Here, the `recipient` and the `message` change, but the process of sending the message is always the same.

To write a re-usable code where only some values change every time we use something called `functions`.

(you don’t have to remember anything; we will google what we need when we need it)

Open <a href="https://google.com" target="_blank">Google</a> and search how to create function in python click on the first result and look at the example. The function will look something like below.

```
def my_function():
  print("Hello from a function")
```

In Python a function is defined using the `def` keyword. No need to remember; you can always google the syntax when you need it.

Let’s change the function name to something useful.
If you remember from part one, naming anything in programming is just like saving a contact on your phonebook. You can call it anything you want; names are just for reference.

```
akash = 9999999999
abc = 8888888888
xyz = 7777777777

def send_message():
  print("Hello from a function")
```


We already know that the only values that will change while sending a message are the `recipient` and the `message text`. We need to find a way to pass values to the function. Let’s as google about it.

Search for how to pass values to function in python
You already know the drill by now, so check out the first result and read it to learn more about functions.
Now let’s update our code to add two arguments to our function.

```
akash = 9999999999
abc = 8888888888
xyz = 7777777777

def send_message(recipient, message_text):
  print("Hello from a function")
```

If you try to run this code, nothing will happen.
Since functions are re-usable code, it does not run by itself until you specifically call it. Just like to send a message on WhatsApp, you have to click on the send icon. Let’s fix that.
We will call the function and provide it two values, contact as recipient and the text we want to send as message text.
(you can again google for how to call a function in python)

```
akash = 9999999999
abc = 8888888888
xyz = 7777777777

def send_message(recipient, message_text):
  print("Hello from a function")

send_message(akash, ‘Hello World’)
```

Run the function now.
You will see the output as “Hello from a function”, because our function currently just prints that text.
Let’s fix that.

```
akash = 9999999999
abc = 8888888888
xyz = 7777777777

def send_message(recipient, message_text):
  print(‘Sending a message…’)
  print(recipient)
  print(message_text)

send_message(akash, ‘Hello World’)
```

Run it now, and if everything goes well, you will see the following output.
```
Sending a message…
9999999999
Hello World
```

That’s roughly how every tiny feature on your phone works.
When you click an icon or a button on your phone, a function runs and executes the task.

## Now you know how to think like a programmer.

Pick up another feature of your phone and try to visualize it using code just like we did above.
If you get stuck, help is just a google search away.
Do not be afraid to use google. Even expert programmers look up google all the time.


> Repetition is how we learn.  
> Repetition is how we learn.  
> Repetition is how we learn. 

You will slowly start to rely less on Google searches.

## You do not need to know everything
Most of the online tutorials I came across burden you at the initial stage with all the information you do not need when starting out.
You do not need to know and remember all data types.
You do not need to understand all the coding terminology and complicated concepts, and I believe knowing more overwhelms you and make programming look a challenging task.

That’s how I learned to program.

> Don’t copy-paste code; read and type out yourself.
> 
> Use less of your memory, more of your brain.
> 
> Rely less on tutorials and more on creativity.

# Introduction

Say hello to a new package called **voix** ! **'Voix'** is a french word which stands for 'Voice'. As the name suggest , It generates voice for you. Just you have to pass a piece of text. Thats it! Let's discover the details.

## Installation

First of all , we need to install it. Right ? To install it , we need this command:
```bash
pip install voix==0.1
```
Now, we are ready to learn it ! Let's go....

# Let's jump into coding

You know, in python , if we want to use any package, we need to import it , first.

So let's do that!

```python
import voix
```

As **voix** has 1 function which is `speak()`, we can import this function only!

```python
from voix import speak
```

# Discovering the '`speak()`' function

Ok! We are ready to get started !

The `speak()` function needs 5 parameters. But 4 of them are optional . We have to pass one parameter to start our work and it is **text**.

Let's implement this to the code.

```python
from voix import speak

speak("Here we will write the text")
```

**Congratulations!** We have generated our first voice! 


## **The Lang Parameter**

You might notice that the voice is generated by an English man. But we don't want it. In this scenario , **lang** parameter comes to play a vital role. We can pass all of these 32 languages listed below as a 'String' . But first let's see the code

```python
from voix import speak

speak("Here we will write the text" , "fr") #here 'fr' means french
```

More specifically, we can write:

```python
from voix import speak

speak(text="Here we will write the text" , lang="fr") #here 'fr' means french
```

Perfect! Now see if your favorite language is in the list

| Supported Language | Key for writing code |
| ------------------ | -------------------- |
| Arabic             | ar                   |
| Bengali            | bn                   |
| Czech              | cs                   |
| Danish             | dn                   |
| Dutch              | nl                   |
| English            | en                   |
| Finnish            | fi                   |
| French             | fr                   |
| German             | de                   |
| Greek              | el                   |
| Gujrati            | gu                   |
| Hindi              | hi                   |
| Hungarian          | hu                   |
| Indonesian         | id                   |
| Italian            | it                   |
| Japanese           | ja                   |
| Kannada            | kn                   |
| Korean             | ko                   |
| Malayalam          | ml                   |
| Polish             | pl                   |
| Portuguese         | pt                   |
| Romanian           | ro                   |
| Russian            | ru                   |
| Slovak             | sk                   |
| Spanish            | es                   |
| Swedish            | sv                   |
| Tamil              | ta                   |
| Telungu            | te                   |
| Thai               | th                   |
| Turkish            | tr                   |
| Ukrainian          | uk                   |
| Vietnamese         | vi                   |


By default the language is **English**

## **The save Parameter**

In some cases, you might want to save the audio. For this, we can use the save parameter. It receive a Boolean (True or False). By default. **Voix** will not save the audio. But manually we can do it. 

Let's see it in the code !

```python
from voix import speak

speak(text="Here we will write the text" , lang="fr" ,save=True) 
```

That's it! Cool ?

## **The FileName Parameter**

If we save the audio, we will see that the audio file is saved with a name callse **default.mp3**. But we don't want that ! We need our own name.

Let's see how can we do this in code. 

```python
from voix import speak

speak(text="Here we will write the text" , lang="fr" ,save=True, fileName="Biiiiig_File_Name")
```

Now, we will see that , the audio file is named as "**Biiiiig_File_Name.mp3**" . 

## **The Translate Parameter**

We have completed all of the features of **Voix** , Now , we will learn the last feature called **Translate**

Can we translate text and generate voice by the translated text using voix ? Surprisingly , the answer is YES !

Now let's see it in the code !

```python
from voix import speak

speak(text="Here we will write the text" , lang="fr" ,translate=True)
```
By the way, I don't want to save the audio file. So I have removed it. Don't be confused !

That's it ! We have completed the package called **Voix**

## Unexpected Problems
Sometimes, **Voix will not work** without internet. So make sure that while **we are running voix , Just turn on the internet**

## **Fun Fact 😅**
Voix is a very small library. It has only 90 lines of code. Whereas, The Documentation readme file has about 150 lines of code. 😅😅

Hope you like the package. Thanks for using it
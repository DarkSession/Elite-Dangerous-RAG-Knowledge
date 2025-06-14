## Recent Community-created Thargoid Link puzzle

Published: 03 Feb 2019 on Canonn (https://canonn.science/news/recent-community-created-thargoid-link-puzzle/)

Content: ### Following is the write-up from LCU No Fool Like One about the recent community-created Thargoid Link puzzle.

Congratulations to **Commander Ethzero** for solving the little puzzle we set to commemorate the departure of Ed Lewis from the Pilot’s Federation. I have been watching with great interest the work you have all been doing to break the code and it was nice to see you **working together in the open** which is very much the ethos of Canonn.

But before I move on to the debriefing I would first like to apologise if anyone was misled about the nature of the task. I had thought that it would be obvious that this was not a genuine message from the Thargoids but I had not anticipated that people’s desire for a true puzzle of this nature would lead them to suspend disbelief and leave some feeling let down.

I assure you that if we ever organise an event of this nature outside of one of our periodic Canonnball events then we will make it clearer that it is indeed community created.

With that apology out of the way I would like to give you a breakdown on how you could have arrived at the solution and the tools you could have used to help you along the way. I will not be revealing the answer but this debriefing will allow you to arrive at the solution very quickly.

###### PLEASE READ NO FURTHER IF YOU WISH TO SOLVE THE PUZZLE ON YOUR OWN

There are a number of clues in the news post that are there to help you solve the puzzle. There are additional clues in the Hutton Orbital Radio Show linked below that will help with filling in some gaps in your knowledge. The main clues are as follows:

http://media.forthemug.com/190131edleaving.mp3

The Clues

- The message was for Ed Lewis
- There was a hidden image of a system in the first part of the message
- The second part of the message is a trinary sequence
- The system in the image is the key to unlocking the second part of the message

The most important part of this task was to convert the trinary sequence into an ascii string.

The alien signal had three tones low medium and high and were grouped into three. A trinity of trinary tits. These are represented with the numerals 1 2 and 3 You could decode these by ear, but the easiest way is to use a spectrum analyser. You can find some details on how to do this here: **[*Spectrogram View – Audacity Help* Manual](https://manual.audacityteam.org/man/spectrogram_view.html)**

If you don’t understand number bases you might find this guide useful: *[**Binary Numbers Explained – Beginners Guide**](http://www.steves-internet-guide.com/binary-numbers-explained/)*

In this instance we made it easy for you by encoding high as 2 medium as 1 and low as 0. However genuine Thargoid messages are binary and counter-intuitively encode high as 0 and low as 1, so a thorough commander would have explored all possibilities.

Once you have transcribed your trinary numbers you can then use this lookup table to work out the ascii numerals.

![](https://canonn.science/wp-content/uploads/2019/02/Table1-300x32.jpg)

The resulting string is gibberish:

```
 vimphkrqeygnibhofsscdfmubiovwnxcut
```

However one of our clues is that the system is the key to unlocking the message so that suggests that the message is a Vigenère cipher. The Vigenère cipher was once known as the unbreakable cyper and it took three centuries to break it. You can find out more here: *[**Vigenère cipher – Wikipedia**](https://en.wikipedia.org/wiki/Vigen%C3%A8re_cipher)*

What you may find surprising is that a number of you came very close to solving the puzzle by simply guessing the content of the message.

The cypher is decoded using the keyword, however if you guess the message you can put the message into a decoder and it will decode the message to show the key. If the words you guess are not at the beginning of the message you can simply pad the front of your guess until you see something that could look like the keyword.

[![](https://canonn.science/wp-content/uploads/2019/02/CanonnDecryptor-1-300x260.jpg)](https://kayahr.github.io/canonn-decryptor/#/?data=N4IgdghgtgpiBcIQBoQEswAcCuAXAzggNqgY64JIC%2BAulUA%3D)

***[Canonn Decryptor Tool](https://kayahr.github.io/canonn-decryptor/#/?data=N4IgdghgtgpiBcIQBoQEswAcCuAXAzggNqgY64JIC%2BAulUA%3D)***

So let’s assume that you have got this far and not been able to guess the message or any parts of its content. You have no other choice than to find out the secret key so you will need to view the hidden message in the file.

Once again you can use the spectrum analysis tool to view the image in the message. A number of commanders did a truly excellent job of this. In fact they did a far better job than I was able to do myself.

The image you uncover will give you some clues about the system you are looking for. You should record as many facts about the system as you can so that you can compare it with potential candidates.

I am not so cruel as to force you to search through the whole EDSM database for matching systems. If you remember the first clue is that the message is somehow connected with Ed Lewis. The audio broadcast on the Gnosis can give you some ideas about what that connection may be.

If that gives you some ideas about potential systems then you should look them up on EDSM to see if they match the image from the audio. Or you could skip that step and just use the names as the keywords in the decryptor and the answer should simply pop out.

I hope that this tutorial has been helpful. Good luck uncovering the message.

***CMDR LCU No Fool Like One***
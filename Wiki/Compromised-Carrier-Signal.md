# Compromised Carrier Signal
Occasionally, local GalNet reports are marked with **\*\*\*Compromised Carrier Signal\*\*\***, indicating that the GalNet system was not able to decrypt the message appropriately. These messages are known to contain "something of interest", but must be decrypted entirely manually, as there is no available tool or process to do so within *Elite Dangerous* itself.^[1]^

## 

Contents

- 1 Decrypting Carrier Signals
    - 1.1 Encryption Types
    - 1.2 Decrypting Morse Code
    - 1.3 Decrypting Letterwise Translation
- 2 References

## Decrypting Carrier Signals

### Encryption Types

The following types of encrypted messages have been found:

- Morse Code
- Letterwise Translation
- ...

### Decrypting Morse Code

### Decrypting Letterwise Translation

This kind of encryption maps every letter to another letter. Numbers are still the same. To decrypt this kind of message you need to know the translation of at least a few letters. 

 	 	 	 		 			 		 		 		 			
*Example for an encrypted message found in Pand system*
 		 	 

```
C F O 2 8 5 T J C G
```

```
F S Z R - C C 1 3 - 1 2 -
```

```
C M B O O J Q L
```

```
N Q L - T G B S -
```

```
E N S B G J T M
```

```
N E T
```

Now, the difficult part is to find out which letter stands for which original letter. So, we need at least a few letters to start with. We presume, that the message contains system coordinates and fortunately that is true. Looking in the vicinity of Pand (where this message was found) there is a system called "CLO 285 SECTOR ZQC C13 12". This matches pretty closely to our message, as we see here:

```
C F O 2 8 5 T J C G F S Z R - C C 1 3 - 1 2
```

```
C L O 2 8 5 S E C T O R Z Q   C C 1 3   1 2
```

Thus, we start with a translation table, which contains this:

| encoded | A | B | C | D | E | F | G | H | I | J | K | L | M |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| shift |  |  | 0 |  |  | -17 | -13 |  |  | -5 |  |  |  |
| decoded |  |  | C |  |  | O/L | T |  |  | E |  |  |  |

| encoded | N | O | P | Q | R | S | T | U | V | W | X | Y | Z |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| shift |  | 0 |  |  | -1 | -1 | -1 |  |  |  |  |  | 0 |
| decoded |  | O |  |  | Q | R | S |  |  |  |  |  | Z |

The row titled *shift* is the difference of the position between the encoded and the decoded letter in the alphabet, considering a wrap around at the first letter A to the last letter Z.

We notice some inconsistencies in this table. For example decoded O is either directly mapped from encoded O or mapped from encoded F. Those differences appear only in encryption of letters in coordinates, such as CLO and ZQC, which seem to have a different encoding rule. This looks more like they are either directly mapped or contain random errors. Consequently, we cannot rely on them entirely.

Now, we can translate more of the remaining message leaving unknown letters open.

```
C M B O O J Q L N Q L - T G B S - E N S B G J T M N E T
```

```
C . . . . E . . . . . - S T . R - . . R . T E S . . . S
```

The message still contains too many missing letters to find the actual information. Looking at the row with the *shift* for each letter in our translation table and ignoring the letters of coordinates, we see that those are all negative prime numbers which are ordered ascending. So, presumable, there are sections in the alphabet with the same shift which is a negative prime. Thus, all letters with yet unknown mapping will belong to one of those sections. For example Q lies between a section with shift -1 and there must be another section with shift -3 left of it. Thus, Q maps either to P (shift -1) or N (shift -3). Thus, for missing letters, we have just a few possible candidates and and can start looking for patterns which might match any english word.

Here M is a good candidate to start of because there are not many letters in english words following a C (first appearance) and S (second appearance). For M we get the candidates L (-1), J (-3) and H (-5), thus H is a reasonable mapping, resulting in CH and SH. Following this procedure we can go on and find other letters, until we found all missing letters, which results in this translation table:

| encoded | A | B | C | D | E | F | G | H | I | J | K | L | M |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| shift |  | -1 | 0 |  | +11 | -17 | -13 |  |  | -5 |  | -5 | -5 |
| decoded |  | A | C |  | P | O/L | T |  |  | E |  | G | H |

| encoded | N | O | P | Q | R | S | T | U | V | W | X | Y | Z |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| shift | -5 | -3/0 |  | -3 | -1 | -1 | -1 |  |  |  |  |  | 0 |
| decoded | I | L/O |  | N | Q | R | S |  |  |  |  |  | Z |

There are some inconsistencies in the table considering the pattern with sections of prime numbers we have found (see mapping for E) but for the most part it works and you finally get this message:

```
C M B O O J Q L N Q L - T G B S - E N S B G J T M N E T
```

```
C H A L L E N G I N G - S T A R - P I R A T E S H I P S
```

The message itself is not an actual sentense, you may note, but it gives a hint on what you have to expect: something with a star, pirates, ships and it is indeed challenging. Good luck!
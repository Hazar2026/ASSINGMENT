# Your Name in Disguise
## Objective
The objective of this activity is to create a secret codename by converting my name into hexadecimal format and my birth year into binary format.
## Flowchart
<img width="1086" height="1448" alt="FLOWCHART" src="https://github.com/user-attachments/assets/8a77324f-66ce-4449-a254-49a48f752ddb" />

## Name Used

My name in lowercase:

```text
hazar zaman
```

## Name to Hexadecimal Conversion

| Character | ASCII Decimal | Hexadecimal |
| --------- | ------------: | ----------- |
| h         |           104 | 68          |
| a         |            97 | 61          |
| z         |           122 | 7A          |
| a         |            97 | 61          |
| r         |           114 | 72          |
| space     |            32 | 20          |
| z         |           122 | 7A          |
| a         |            97 | 61          |
| m         |           109 | 6D          |
| a         |            97 | 61          |
| n         |           110 | 6E          |

## Final Hexadecimal Codename

```text
68617A6172207A616D616E
```

## Birth Year Used

Birth year:

```text
2004
```

## Birth Year to Binary Conversion

To convert 2004 from decimal to binary, I divided by 2 and kept track of the remainders.

| Division | Quotient | Remainder |
| -------- | -------: | --------: |
| 2004 ÷ 2 |     1002 |         0 |
| 1002 ÷ 2 |      501 |         0 |
| 501 ÷ 2  |      250 |         1 |
| 250 ÷ 2  |      125 |         0 |
| 125 ÷ 2  |       62 |         1 |
| 62 ÷ 2   |       31 |         0 |
| 31 ÷ 2   |       15 |         1 |
| 15 ÷ 2   |        7 |         1 |
| 7 ÷ 2    |        3 |         1 |
| 3 ÷ 2    |        1 |         1 |
| 1 ÷ 2    |        0 |         1 |

The remainders are read from bottom to top.

## Final Binary Birth Year

```text
11111010100
```

## Final Secret Codeword

My final secret codeword is my hexadecimal name plus my binary birth year.

```text
68617A6172207A616D616E-11111010100
```

## Challenges

The main challenge was making sure my name was converted to lowercase before changing it into hexadecimal. Another challenge was remembering to include the space between my first and last name, because a space also has an ASCII and hexadecimal value. Converting the birth year to binary also required careful division by 2 and reading the remainders from bottom to top.

> WAV is a proud soldier of Bunker 8, responsible for defending the west border of his country. They were attacked by the enemy at night without any prior information and hence were hit hard. WAV immediately tried contacting Headquarters but his message got corrupted in between and now the Headquarters are unable to respond to their soldiers' message.
> 
> Help the Headquarters to decipher the message and help their men! The answer format is CTF{message}, the message exactly in the same format as obtained, no spaces.

First fix the file signature to match that of wav format, the first four bytes should be `52 49 46 46`. Use this [spectrum analyser](https://academo.org/demos/spectrum-analyzer/) to get the flag.

The flag is `CTF{WE-NEED-REINFORCEMENTS}`

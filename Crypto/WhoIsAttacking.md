# Who is Attacking?

> the ~~international~~ french ~~space~~ water station was broadcasting a secret [message](https://drive.google.com/file/d/1ZFc7sx_bNt3vJ_8KZW9n_M-bysNC2SsC/view) to its headquarters. since the message was being broadcasted very Slowly, someone Scanned the message using their very old TeleVision but all they could hear were some distorted noises.....
> 
> Submit after enclosing inside CTF{} and separate the words with an underscore ( _ )

Follow the instructions on this [article](https://ourcodeworld.com/articles/read/956/how-to-convert-decode-a-slow-scan-television-transmissions-sstv-audio-file-to-images-using-qsstv-in-ubuntu-18-04) to turn the audio file into an image. Decrypt the maritime signal flags into text. The image reads `uz1g4 1n sl74vf1fy`. Decode using Vigenere with key `sstv`.

The flag is `CTF{ch1n4_1s_at74ck1ng}`

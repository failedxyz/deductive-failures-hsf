# 500 Where is My Key

> Well this is embarrassing. I was writing a program that I could use to send encrypted messages between my friend and me, but somehow I managed to lose my key and the original message that I sent to my friend. I have a message and it's encrypted version from when I still had the key, but I really want to get back the second message that I sent. Can you help me?
>
> where_is_my_key_95e256e61968a6cd6faf7c4a9a2ff35c5849a951.zip

So there's an encryption algorithm in `encryptor.c`, which encrypted `message1` to `message1.enc` and a missing `message2` to `message2.enc`. And we're trying to find the original `message2`.

To approach this, we'll figure out how `message1` is encrypted to `message1.enc`, and the key used, and then reverse the process for `message2.enc`.

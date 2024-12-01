Min egen bitmap er genereret fra siden random.org, scroll til:
Lists and Strings and Maps, Oh My!
og click på Bitmaps in black and white
link:
https://www.random.org/bitmaps/?format=png&width=64&height=64&zoom=1
download bitmap

kør scriptet:
python3 images_xor.py -p my_bitmap/64x64.jpeg -k my_bitmap/bitmaps.png -c my_bitmap/result.png

eller:
python3 images_xor.py -p example/plaintext.jpeg -k example/key.gif -c example/result.png

eller:
python3 images_xor.py -p decrypting_otp/ciphertext.gif -k decrypting_otp/key.gif -c decrypting_otp/decrypted.png

Ændre XOR operationen til AND eller OR i linjen:
ciphertext = ImageChops.logical_xor(plaintext, key)

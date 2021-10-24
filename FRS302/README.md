# FU Secathon Writeup

2021 - Forensics category

# FRS301

## Brief

The challenge is an audio that have morse code in it, but it also contains background noise and I couldn't seperate the sound.

We can note it down manually by viewing the spectrogram of the audio in Audacity. Then decode it in [dcode.fr](https://www.dcode.fr/morse-code)

[Download file here](https://github.com/n3ddih/FuSec2021_Writeup_FRS/raw/main/FRS302/echoslambyjava.wav)

## Details

Open the wav file and view the spectrogram of it.

![image](https://user-images.githubusercontent.com/80664686/138596966-0b0132ac-987d-4d73-9633-b4166f79e4a9.png)

As you can see, there are lines that represent the morse audio.

We can manually view and write down the morse code. 

> Short line for a *(.)*</br>
> Long line for a *(-)*</br>
> Short gap for a *space*</br>
> Long gap for a *(/)*

**Bonus**: you could set datas in *spectrogram settings* like below for easier inspection.

![image](https://user-images.githubusercontent.com/80664686/138599249-6135611c-1c8e-45a2-900e-8c7cfa1605c1.png)

> Morsecode:</br>
> .-.. .- -.- .- -../-- .- - .- - .- --./-. --- .-. -- .- .-.. .. -./-. --- .-. -- .- .-.. .. -./. -.-. .... ---/... .-.. .- --/-... -.--/.--- .- ...- .-/--- -.--/--- -.--/--- -.--/--- -.--/--- -.--/--- -.--/--- -.--/--- -.--/--- -.--

The morse can be decode using [dcode.fr](https://www.dcode.fr/morse-code)

![image](https://user-images.githubusercontent.com/80664686/138600380-1a9b218e-1f45-49ec-a61d-7a1102964574.png)

> Flag: FUSEC{LAKADMATATAGNORMALINNORMALINECHOSLAMBYJAVAOYOYOYOYOYOYOYOYOY}

# For Sale Private SOFT BrainWords $300

## Find Lost Bitcoin Passphrases (Brainwallet)
Search passphrases on the fastest program in the world<br>
18,972 passphrases were found, an estimated 5,000 passphrases are lost<br>
They were found on a processor with a maximum speed of 100,000 pasdphrases per second.<br>
Speed RTX 4090 = 360,000,000 passphrases/sec. It's 3600 times faster.<br>
The fact that one 4090 GPU runs in 24 hours is a legendary CPU program in 10 years.<br>

![brainwallet gpu](https://github.com/phrutis/BrainWords_For_Sale/assets/140947743/5f2d14ba-9eaf-49ad-a91f-eb20640d1ce9)

**To buy the program, write in telegram** @phrutis

| GPU card | --bits | Speed |
|----------|----|-------------|
| 4090     | 24	| 360 Mkeys/s |
| A100     | 24 | 180 Mkeys/s |
| A6000    | 24 | 180 Mkeys/s |
| 3090     | 24 | 180 Mkeys/s |
| 3080 Ti  | 24 | 170 Mkeys/s |
| 3080     | 24 | 150 Mkeys/s |
| 3070 Ti  | 24 | 120 Mkeys/s |
| 3070     | 24 | 110 Mkeys/s |
| 3060     | 24 | 70 Mkeys/s |
| 2080 S   | 24 | 70 Mkeys/s |
| 2070     | 24 | 50 Mkeys/s |

How to search for old lost passphrases:<br>
Default alphabet: ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789 .,'!-

-v - verbose output<br>
--bits 16 or 20 or 24
--inputAddress addresses.txt - file with addreses<br>
--inputPhrase dictionary.txt - file with phrases and pass<br>
-d ? (GPU card number, id)<br>
--eth (ETH address search) --inputAddress addrEth.txt default mode: BTC, single sha256

#### For ETH:
--eth - single keccak<br>
--camp2 - keccak*2031<br>
^^^ two options could be used together<br>
--ethsha256 - sha256 for ETH<br>
--root - specifies prefix for your word<br>
--suffix - number o combimnation to start from<br>

Run: ```BrainWords.exe -v --eth --root "Hello word " --suffix 708550400 --inputAddress addresses-Eth.txt```


Prefix + Combinations<br>
TestA -> TestB -> TestC -> Testzzzzz -> Testzzzzzzzzzzzzzz<br>
Run ```BrainWords.exe -v --bits 24 --root Test --suffix 0 --inputAddress addresses.txt -d 0```

Test test A -> Test test B -> Test test C -> Test test zzzzz -> Test test zzzzzzzzzzzzzz<br>
Run ```BrainWords.exe -v --bits 24 --root "Test test " --suffix 0 --inputAddress addresses.txt -d 0```

Combinations + Suffix (v0.8 only)<br>
A@gmail.com -> B@gmail.com -> C@gmail.com -> zzzzz@gmail.com -> zzzzzzzzzzzzzz@gmail.com<br>
Run ```BrainWords.exe -v --bits 24 --rootsuffix @gmail.com --suffix 0 --inputAddress addresses.txt -d 0```

A Test test -> B Test test -> C Test test -> zzzzz Test test -> zzzzzzzzzzzzzz Test test<br>
Run ```BrainWords.exe -v --bits 24 --rootsuffix " Test test" --suffix 0 --inputAddress addresses.txt -d 0```

Finding passphrases from a text file<br>
Run ```BrainWords.exe -v --inputPhrase dictionary.txt --inputAddress addresses.txt -d 0```

Hashcat + BrainWords (streaming from an external character generator)<br>
Run ```hashcat.exe --stdout -a 3 --increment ?u?l?l?l?d?d?d | BrainWords.exe -v --inputIn --inputAddress addresses.txt -d 0```

**Linux:**

For ubuntu (linux), be sure to convert the address database to Unix format.<br> 
This will remove the ^M from the end of addresses<br>
sudo apt update<br>
sudo apt install -y dos2unix<br>
dos2unix addresses.txt<br>

Run ```chmod +x BrainWords```<br>
Run ```./BrainWords -v --bits 24 --root Test --suffix 0 --inputAddress addresses.txt -d 0```

**Hashcat**
<br>
Run ```./hashcat.bin --stdout -a 6 dictionary.txt --increment ?d?d?d?d | ./BrainWords -v --inputIn --inputAddress addresses.txt -d 0```<br>
or<br>
Run ```./hashcat.bin --stdout -a 3 --increment ?u?l?l?l?d?d?d | ./BrainWords -v --inputIn --inputAddress addresses.txt -d 0```<br>
(If you need more speed, make a copy of the hashcat folder)
<hr>

### Frequently asked Questions

**How to buy the program?**
<br><br>
Write @phrutis in telegram.<br>
Payment in BTC<br>
After payment you will receive 2 zip archives
First v0.7<br>
Second v0.8<br>
The difference in v0.8 is added --rootsuffix<br>
You can also specify the bit depth for the bloom filter.<br>
Otherwise everything is the same.<br>
There is also a short instruction inside the archives.<br>
After the purchase, I will help with the launch, we will check the performance and other issues.
<hr>

**Why did the program freeze at startup?**
<br><br>
She didn't hang up! Program start 3090 --bits24 (10 min.)<br>
The program creates tables and downloads to the device<br>
One card requires 4GB or more of RAM to work.<br>
The consumption depends on the size of the table (--bits) and the size of the address file.<br>
<hr>

**What address formats can be uploaded?**
<br><br>
BTC bc.., 3.., 1.., or ETH in a text file from a new line<br>
It is recommended to use only OLD addresses 1... from $2
<hr>

**How to continue searching after stopping the program?**
<br><br>
The program saves the position<br>
You can start from any position by specifying --suffix 1234567
<hr>

**How to start with 9 characters?**
<br><br>
Count the number of characters in the alphabet and choose the one you need.<br>
Example 9 characters (alphabet 64 characters)<br>
64 * 64 * 64 * 64 * 64 * 64 * 64 * 64 = 281474976710656<br>
Use --suffix 281474976710656<br>
<hr>

**How do I search for 9 characters on 50-150 cards?**
<br><br>
Divide the desired range into parts (into cards)<br>
18014398509481984 (9) - 281474976710656 (8) = Difference 17732923532771328<br>
17732923532771328 / 50 (cards) = 354658470655426

GPU 0 281474976710656<br>
GPU 1 281474976710656 + 354658470655426 = --suffix 636133447366082<br>
GPU 2 636133447366082 + 354658470655426 = --suffix 990791918021508<br>
GPU 3 990791918021508 + 354658470655426 = --suffix 1345450388676934<br>
...<br>
GPU 50 17378265062115902 + 354658470655426 = --suffix 17732923532771328<br>
<hr>

**Explain what we are looking for?**
**How it works? What's this?**
<br><br>
Here is a good example of work for you.<br>
Enter passphrase: fhqyqzhao123 pay attention to the address 1MVFUmYLKmLyC1m3WfyHkEJTZfoHjwDeXE<br>
The difference is that instead of requests to the blockchain.<br>
The program checks against the database of addresses with a positive balance.
<hr>

**What is a brain wallet?**
<br><br>
These are passwords or phrases converted to sha256; the output is a private key to the address.<br>
At the address, people stored coins there, a passphrase in their heads.<br>
This method was used 10-15 years ago. At that time, coins were worth almost nothing.<br>
Passwords were lost and forgotten. Do you remember your password 12 years ago? Are you sure?<br>
One character, dot or register is wrong and the entire wallet is lost. There is no restore button.<br>
Look for more information about brain wallet on the Internet.
See hire generstion [https://brainwalletx.github.io](https://brainwalletx.github.io)
<hr>

**What does Brain Wallet look like?**
<br><br>
Were there any finds at all?
<br><br>
Here is a white list of passwords, phrases, balances, study<br>
https://privatekeyfinder.io/brainwallet/bitcoin/
<hr>

**Multigpu program?**
<br><br>
The program is not multigpu. For each card, indicate your id<br>
-d 0 or -d 1 ... -d 11<br>
<hr>

**What does Brain Wallet look like?**
**Were there any finds at all?**
<br><br>
Here is a white list of passwords, phrases, balances, study
https://privatekeyfinder.io/brainwallet/bitcoin/
<hr>

**Why does the program use a lot of RAM?**
<br><br>
The program creates the necessary tables and stores them in memory.
<hr>

**Does the program require an internet connection?**
<br><br>
No, the program is looking for the key offline.
<hr>

**The program is sold with source code?**
<br><br>
Yes, the program is sold with original source code v0.7 and new v0.8 and instructions
<hr>

**How to change the alphabet in the program?**
<br><br>
Yes, open the file **Kernel.cuh** insert your alphabet.<br>
The program only accepts en + numbers and symbols

#define ALPHABET_LEN 68<br>
const char ALPHABET[69] = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789 .,'!-";<br>
__device__ __constant__ char _ALPHABET[69] = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789 .,'!-";<br>
ALPHABET_LEN the exact number of characters in the alphabet<br>
_ALPHABET[the exact number of characters in the alphabet + 1]

#define ALPHABET_LEN 36<br>
const char ALPHABET[37] = "0123456789abcdefghijklmnopqrstuvwxyz";<br>
__device__ __constant__ char _ALPHABET[37] = "0123456789abcdefghijklmnopqrstuvwxyz";<br>
<hr>

**How to compile a program?**
<br><br>
ubuntu 20.04 CUDA 11.7 (for RTX 4090 CUDA 12.2)<br>
Run: ```make```

vast.ai<br>
Template: cuda:12.0.1-devel-ubuntu20.04<br>

Image: nvidia/cuda:12.0.1-devel-ubuntu20.04<br>

Image CUDA version:<br>
Incompatible images hidden<br>
Launch Type: jupyter<br>


Windows use VS2019 + install CUDA 11.7 (for RTX 4090 CUDA 12.2)
<hr>

**How can I make sure that the program does not stop after it finds it?**
<br><br>
Open the main.cu file using a text editor<br>
Line 1100 return true; do this //return true; (ETH addresses)<br>
Line 1124 uncompResult = true; o this //uncompResult = true; (for P2PKH Legacy 1.. Uncompressed)<br>
Line 1140 compResult = true; o this //compResult = true; (for P2PKH Legacy 1.. Compressed)<br>
Line 1155 bech32Result = true; o this //bech32Result = true; (for bc.. addresses)<br>
Line 1170 compResult = true; o this //compResult = true; (for P2SH addresses 3..)
<hr>


**In what modes is the program looking for?**
<br><br>
She is looking for everyone at once.<br>
Addresses 1 (uncompressed + compressed), addresses 3... in bc...
<hr>

**I have a RTX 3060 TI card, and I have a low speed, how can speed up?**<br>
In the new drivers for 30xx Ti, a limiter is installed that slows down the speed by half.<br>
You need to download the old driver from six months ago. 496.13<br>
Delete the new driver, install the old driver, the speed will increase x2<br>
After searching, you can install new drivers.<br>
<hr>

**What arguments are there in the program?**
<br><br>
```-v``` Display the generation position in the program window<br>
```-b``` Number of gpu blocks (default set automatically)<br>
```-t``` Number of gpu cores (default set automatically)<br>
```--bits``` Number of bits to generate table 8, 16, 20, 24<br>
```--fstatus``` File name status (default fileStatus.txt)<br>
```--inputAddress``` List of addresses of BTC or ETH in a tex file from a new line<br>
```--inputPhrase``` Name of a text file with a list of BTC or ETH addresses starting on a new line<br>
```--inputIn``` Receive a stream of phrases from an external generator<br>
```--iteration``` Number of iterations SHA256<br>
```--eth``` Enable mode ETH (default BTC)<br>
```--camp2``` Enable search mode for camp2 (keccak*2031) ETH addresses<br>
```--ethsha256``` sha256 for ETH<br>
```--root``` Fixed part in generation ```--root 1234``` or ```--root " 1234 1234"``` with space<br>
```--suffix``` Number o combimnation to start from ```--suffix 0```
```-d``` number of the required gpu ```-d 0``` or ```-d 1```
<hr>

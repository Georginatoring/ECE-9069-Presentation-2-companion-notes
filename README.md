# RFID replay and cloning exploits!

## By: George Bousygine
###  March 22, 2021
---

## **Background**  

### **What is RFID? [[1]](https://www.abr.com/what-is-rfid-how-does-rfid-work/)**
Stands for "radio-frequency identification". Working on radio waves to automatically identify an object. 

Different types of technology that use RFID: 

* Inventory management
*  Asset tracking
*  Personnel tracking
*  Controlling access to restricted areas
*  ID Badging
*  Supply chain management
*  Counterfeit prevention 

### *How does it work?*
There are active and passive RFIDs [read more](https://www.atlasrfidstore.com/rfid-insider/active-rfid-vs-passive-rfid#:~:text=Once%20the%20tag%20is%20read,back%20to%20the%20RF%20system.&text=Hard%20RFID%20tags%20are%20durable,metal%2C%20ceramic%20and%20even%20rubber.)

(we will only focus on passive)

There are 3 Families:

[Read more](https://www.atlasrfidstore.com/rfid-beginners-guide/) [2] 
1. Low Frequency (LF) using 125-134 KHz
2. High Frequency (HF) using 13.56 MHz
3. Ultra High Frequency (UHF) 433 MHz



The RFID tags contain an IC powered through an induction coil and transfers data to a receiving antenna through radio waves.

![diagram](https://www.electronicshub.org/wp-content/uploads/2013/07/Functioning-Principle-of-RFID-Device.png)





## **Vulnerability**

Since the data is transferred through airwaves, it is vulnerable for replay and cloning (and some cases man-in-the-middle attacks [3]).

There are a few tools that can be used to maliciously read and clone RFID tags.
### *RFID Tools*

**Card Copier Writer Duplicator (LF)**

![diagram](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSCL6cAH4VN4qzJVZIT0h3huTkpe4EjGIXExw&usqp=CAU)

**Proxmark3 (HF)**

![diagram](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRpjDVRPJ8c_1i4t9KRFN8Wp9HV3sop6Ktvmw&usqp=CAU)

**RFID READER SNOOPS CARDS FROM 3 FEET AWAY**  [read more](https://hackaday.com/2013/11/03/rfid-reader-snoops-cards-from-3-feet-away/)

![diagram](https://hackaday.com/wp-content/uploads/2013/11/rfidlongrangehack.png?w=670)

An individual can get access to these tags by being in close proximity to the device, tapping the reader against it (data transfer can happen through clothes), or physically having access to the device for a short period of time. It takes a few milliseconds to read all the data on the chip and once the data is captured, it can be cloned right away or decrypted through hacking tools at a later time. [4]

[Step-by-step Tutorial: How to Copy or Clone Access Cards and Key Fobs](https://www.getkisi.com/blog/how-to-copy-access-cards-and-keyfobs)

## **Ways to prevent**

* Using NFC (a subset of RFID) for credit cards and or other sensitive data  [read more](https://www.pcworld.com/article/2938520/nfc-security-3-ways-to-avoid-being-hacked.html#:~:text=NFC%2C%20based%20on%20contactless%20smartcard,and%20adding%20security%20and%20privacy.)

### *blocker*
1. RFID blocking wallet
2. RFID blocking card


### **Reference**


[1] What is rfid and how does rfid work? - ab&amp;r®. (2021, February 15). Retrieved March 21, 2021, from [Link](https://www.abr.com/what-is-rfid-how-does-rfid-work/). 


[2] RFID Frequncies. (n.d.). Retrieved March 21, 2021, from  [Link](https://www.atlasrfidstore.com/rfid-beginners-guide/)

[3] Anderson, R. (n.d.). RFID and the Middleman. Retrieved from [Link](https://www.cl.cam.ac.uk/~rja14/rfid-fc07.pdf)

[4] R. Jain, D. Kumar Chaudhary and S. Kumar, "Analysis of Vulnerabilities in Radio Frequency Identification (RFID) Systems," 2018 8th International Conference on Cloud Computing, Data Science & Engineering (Confluence), Noida, India, 2018, pp. 453-457, doi: 10.1109/CONFLUENCE.2018.8442623.

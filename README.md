# Email Attachment Analysis

<h2>Description</h2>
In this email attachment analysis, I examine a suspicious attachment, generate a sha256 hash, and use virustotal and talosintelligence to investigate it. 
<br />


<h2>Languages and Utilities Used</h2>

- <b>Linux CLI</b>
- <b>Virustotal</b>
- <b>Talosintelligence</b>


<h2>Environments Used </h2>

- <b>Unbuntu</b> 

<br />
<br />
Ssaved attachment as iso file in directory from suspicious email.  

![1) save suspicious attachment as iso file](https://github.com/user-attachments/assets/55a61f21-99b4-4042-9672-76765575caa6)

<br />
<br />
Use DidierStevensSuite emldump.py tool from github. 

![2) using didierstevenssuite emldump python script](https://github.com/user-attachments/assets/ccd77de7-2e54-495b-9c8e-5574e390f9a3)

<br />
<br />  
Help option for flags to use in email dump. 

![3) how to use emldump tool](https://github.com/user-attachments/assets/08069dc6-0e0c-4c79-803a-2f416bdab797)

<br />
<br />
Calling the email dump tool, selecting the 4th option, and dumping the contents into a "quotation.iso" file in current directory.

![4) using tool to extract attachment into an iso file](https://github.com/user-attachments/assets/3fde4dd3-5509-4d7a-82fd-4870ba05fff9)

<br />
<br />
Next I generated a sha256, md5, and sha1 hash of the attachment iso file. 

![5) hash generation](https://github.com/user-attachments/assets/333262ab-601f-4555-9a49-51eda0cdbd85)

<br />
<br />
Running a python ioc tool from a previous task also generates file hashes from the attachment. 

![6) using malwarecube ioc tool extracts attachment and hashes safer](https://github.com/user-attachments/assets/7e43c0bf-603b-4122-bf9d-503d8dedd865)

<br />
<br />
Checking the sha256 hash in virustotal shows the attachment is malicious.

![7) virustiotal output](https://github.com/user-attachments/assets/558a4e57-43c9-42ef-9655-5a0f2ccd1890)

<br />
<br />
Lastly, checking the sha256 in talosintelligence shows the attachment is also malicious. 

![8) talos verdict](https://github.com/user-attachments/assets/420f5b22-5e08-4764-93b9-c8ec412c9872)
<br />
<br />

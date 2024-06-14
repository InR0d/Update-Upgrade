# Update-Upgrade
Day 5 - Cybersecurity and Ethical Hacking
SUDO Daily Challenge: Perform a Brute-Force Attack with John the Ripper in Kali Linux to Crack a Password from a Secured File
In this challenge, you will have the opportunity to perform a brute-force attack using the John the Ripper password cracking tool in Kali Linux to crack a password from a secured pdf document. This exercise focuses on utilizing a powerful password cracking tool within a specialized penetration testing operating system. By following the provided procedure and utilizing the necessary materials, you will gain practical experience in using Kali Linux and John the Ripper to crack a password and understand the implications of weak passwords.

Objectives:
1.	Learn the concept of brute-force attacks and how they can be used to crack passwords.
2.	Develop practical skills by using Kali Linux and the John the Ripper password cracking tool to attempt password recovery.
3.	Explore the vulnerabilities associated with weak passwords and the importance of strong password policies.
4.	Engage in a controlled environment to crack a password for educational purposes and to highlight security weaknesses.
5.	Assess the potential impact of password vulnerabilities and reinforce the importance of secure password practices.

Materials Needed:
1.	Kali Linux operating system (available for download from the official website).
2.	Secured file with a password-protected format (e.g., encrypted ZIP file, password-protected document).
3.	John the Ripper password cracking tool pre-installed in Kali Linux.
4.	Wordlists or dictionaries containing common passwords or custom password lists for the brute-force attack.

Procedure:
1.	Obtain the file that requires a password for access or extraction and ensure it is compatible with John the Ripper.
2.	Start your computer with Kali Linux or set up a virtual machine with Kali Linux installed.
3.	Store the document in Kali Linux Desktop.
4.	Launch the Terminal application in Kali Linux to execute command-line operations.
5.	Use the Terminal to navigate to the directory where the secured file is located.
	   	cd Desktop
7.	Use the Terminal to install necessary tools. Ensure that John the Ripper and Perl are installed on your system.
      sudo apt update	     	  
			sudo apt install john perl     		 	
8.	Extract the hash from the PDF. Use the pdf2john.pl script to extract the hash from the PDF file.
			locate pdf2john.pl									
			perl /usr/share/john/pdf2john.pl CrackThis.pdf > hash.txt		
9.	Crack the Password with John the Ripper. Run John the Ripper:
			john --format=pdf --wordlist=/usr/share/john/password.lst hash.txt
10.	Once John has finished cracking, view the cracked password with: 
			john --show hash.txt
11.	Enter the cracked password to the pdf document.
12.	Reflect on the cracked passwords and analyze their strength and implications. Consider the effectiveness of password policies and the need for stronger password practices.
13.	Evaluate the effectiveness of the password security measures in place and identify areas for improvement.
14.	Always conduct password cracking activities in a controlled and ethical manner, adhering to applicable laws and regulations.

Explanation of Commands

	•	perl /usr/share/john/pdf2john.pl CrackThis.pdf > hash.txt
		This command extracts the hash from the PDF file and saves it to hash.txt.
	
	•	john --format=pdf --wordlist=/usr/share/john/password.lst hash.txt
		This command runs John the Ripper using the PDF hash format and the default password.lst wordlist against the extracted hash.
	
	•	john --show hash.txt
		This command displays any cracked passwords found by John the Ripper.


Requirements:
1.	Familiarity with Kali Linux and its command-line interface.
2.	Understanding of password cracking concepts and techniques.
3.	Basic knowledge of ethical hacking principles and legal boundaries.
4.	Access to a secured file with a password-protected format for testing purposes.
5.	Installation of Kali Linux on your computer or a virtual machine.
6.	Availability of wordlists or dictionaries for the brute-force attack.
7.	Patience and perseverance, as password cracking can be time-consuming.
8.	Awareness of legal and ethical responsibilities in conducting password cracking activities.

Note: Performing password cracking activities should always be done with proper authorization and within a legal and controlled environment. Ensure that you have the necessary permissions and adhere to applicable laws and regulations.


[D5S2 Final Challenge 2024.pdf](https://github.com/user-attachments/files/15839622/D5S2.Final.Challenge.2024.pdf)

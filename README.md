# Update-Upgrade
<h1> Day 5 - Cybersecurity and Ethical Hacking </h1>
<h3>SUDO Daily Challenge: </h3> 
<h4>Perform a Brute-Force Attack with John the Ripper in Kali Linux to Crack a Password from a Secured File.</h4>
<p>In this challenge, you will have the opportunity to perform a brute-force attack using the John the Ripper password cracking tool in Kali Linux to crack a password from a secured pdf document. This exercise focuses on utilizing a powerful password cracking tool within a specialized penetration testing operating system. By following the provided procedure and utilizing the necessary materials, you will gain practical experience in using Kali Linux and John the Ripper to crack a password and understand the implications of weak passwords.</p>
<h3>Objectives:</h3>
<ol>
	<li>Learn the concept of brute-force attacks and how they can be used to crack passwords.</li>
	<li>Develop practical skills by using Kali Linux and the John the Ripper password cracking tool to attempt password recovery.</li>
	<li>Explore the vulnerabilities associated with weak passwords and the importance of strong password policies.</li>
	<li>Engage in a controlled environment to crack a password for educational purposes and to highlight security weaknesses.</li>
	<li>Assess the potential impact of password vulnerabilities and reinforce the importance of secure password practices.</li>
</ol>
<h3>Materials Needed:</h3>
<ol>
	<li>Kali Linux operating system (available for download from the official website).</li>
	<li>Secured file with a password-protected format (e.g., encrypted ZIP file, password-protected document).</li>
	<li>John the Ripper password cracking tool pre-installed in Kali Linux.</li>
	<li>Wordlists or dictionaries containing common passwords or custom password lists for the brute-force attack.</li>
</ol>
<h3>Procedure:</h3>
<ol>
	<li>Obtain the file that requires a password for access or extraction and ensure it is compatible with John the Ripper.</li>
	<li>Start your computer with Kali Linux or set up a virtual machine with Kali Linux installed.</li>
	<li>Store the document in Kali Linux <b>Desktop.</b></li>
	<li>Launch the Terminal application in Kali Linux to execute command-line operations.</li>
	<li>Use the Terminal to navigate to the directory where the secured file is located.<pre><code>cd Desktop</code></pre></li>
	<li>Use the Terminal to install necessary tools. Ensure that John the Ripper and Perl are installed on your system.<pre><code>
sudo apt update	     	  
sudo apt install john perl   
	</code></pre></li>
	<li>Extract the hash from the PDF. Use the pdf2john.pl script to extract the hash from the PDF file.</li>
	<li><pre><code>perl /usr/share/john/pdf2john.pl CrackThis.pdf > hash.txt</code></pre></li>
	<li>Crack the Password with John the Ripper. Run John the Ripper:<pre><code>
john --format=pdf --wordlist=/usr/share/john/password.lst hash.txt
	</code></pre></li>
	<li>Once John has finished cracking, view the cracked password with: <pre><code></code>
john --show hash.txt
	</pre></li>
	<li>Enter the cracked password to the pdf document.</li>
	<li>Reflect on the cracked passwords and analyze their strength and implications. Consider the effectiveness of password policies and the need for stronger password practices.</li>
	<li>Evaluate the effectiveness of the password security measures in place and identify areas for improvement.</li>
	<li>Always conduct password cracking activities in a controlled and ethical manner, adhering to applicable laws and regulations.</li>
</ol>
<h3>Explanation of Commands</h3>

	•	perl /usr/share/john/pdf2john.pl CrackThis.pdf > hash.txt
		This command extracts the hash from the PDF file and saves it to hash.txt.
	
	•	john --format=pdf --wordlist=/usr/share/john/password.lst hash.txt
		This command runs John the Ripper using the PDF hash format and the default password.lst wordlist against the extracted hash.
	
	•	john --show hash.txt
		This command displays any cracked passwords found by John the Ripper.

<h3>Requirements:</h3>
<ol>
	<li>Familiarity with Kali Linux and its command-line interface.</li>
	<li>Understanding of password cracking concepts and techniques.</li>
	<li>Basic knowledge of ethical hacking principles and legal boundaries.</li>
	<li>Access to a secured file with a password-protected format for testing purposes.</li>
	<li>Installation of Kali Linux on your computer or a virtual machine.</li>
	<li>Availability of wordlists or dictionaries for the brute-force attack.</li>
	<li>Patience and perseverance, as password cracking can be time-consuming.</li>
	<li>Awareness of legal and ethical responsibilities in conducting password cracking activities.
</li>
</ol>
<p>Note: Performing password cracking activities should always be done with proper authorization and within a legal and controlled environment. Ensure that you have the necessary permissions and adhere to applicable laws and regulations.</p>

[D5S2 Final Challenge 2024.pdf](https://github.com/user-attachments/files/15839622/D5S2.Final.Challenge.2024.pdf)

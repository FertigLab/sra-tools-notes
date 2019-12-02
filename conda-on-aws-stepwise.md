How to install sra-tools+salmon onto an AWS instance
--------------------------------

By Rebecca Sansale <rebecca.sansale@gmail.com>

1. Open terminal
2. Run in terminal: 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; `ssh -i "name_of_key.pem" username@ec2-instance.amazonaws.com` 

3. Find the correct version of miniconda you want to download (Sasha prefers the 3rd version). You can find the versions with links to download here: <https://repo.continuum.io/miniconda/>. You want to use “Miniconda3-4.7.12.1-Linux-x86_64.sh” . Hover over this link and copy the link. The link should look something like this: <https://repo.continuum.io/miniconda/Miniconda3-4.7.12.1-Linux-x86_64.sh>. 4.7.12.1 is the version of conda script; Linux-x86_64 is the target platform.  
4. Now that you have the version of miniconda picked out, and say <https://repo.continuum.io/miniconda/Miniconda3-4.7.12.1-Linux-x86_64.sh> is or the link to your desired miniconda version, go back to terminal and run: 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; `wget https://repo.continuum.io/miniconda/Miniconda3-4.7.12.1-Linux-x86_64.sh`

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; if everything went correct, now you have the script downloaded; now run it:

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; `bash Miniconda3-4.7.12.1-Linux-x86_64.sh`

5. This is going to prompt you with a few questions, answer “yes”
6. Terminate your current terminal session
7. Open terminal and repeat step 1 to enter your AWS instance once again
8. To install sra-tool, run in terminal: 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; `conda install -c bioconda sra-tools`

9. To install salmon, run in terminal: 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; `conda install -c bioconda salmon`

<h1>Qualys Vulnerability Management Home Lab</h1>


<h2>Description</h2>
This project involves the deployment and utilization of Qualys Vulnerability Management tools to identify and remediate vulnerabilities in virtual machines, with the goal of improving overall system security and reducing potential attack vectors.
<br />


<h2>Program walk-through:</h2>

<p align="center">
Pre-Set up Windows 10 Machine that we will be using for Vulnerability scan: <br/>
<img src="https://i.postimg.cc/fL8hF1Lq/Image-1.png" height="80%" width="80%" />
<br />
<br />

<p align="Center">
Download outdated VLC software and in this lab we will be using VLC 1.1.1 <br/>
<img src="https://i.postimg.cc/sXjM5FqT/Image-2.png" height="80%" width="80%" />
<br />
<br />

<p align="Center">
Download outdated release of Firefox browser, I will be using 103.0 release for this lab <br/>
<img src="https://i.postimg.cc/qBY7vCJb/Image-3.png" height="80%" width="80%" />
<br />
<br />

<p align="Center">
Select the preferred language and download .exe file <br/>
<img src="https://i.postimg.cc/CKPRCr0Y/Image-4.png" height="80%" width="80%" />
<br />
<br />
  Pre-Requisite - Sign up for a free Qualys account before proceeding with the next step.
  <br />
<br />
<p align="center">
Once logged in, download a virtual scanner: <br/>
<img src="https://i.postimg.cc/Znh466W4/Image-5.png" height="80%" width="80%" />
<br />
<br />

<p align="Center">
Click start Wizard and follow the prompt, input the name of the virtual scanner and then download .ova file that we will import to Virtual box  <br/>
<img src="https://i.postimg.cc/SxjF2ggc/Image-6.png" height="80%" width="80%" />
<br />
<br />

<p align="Center">
Open Virtual box and Import Virtual appliance using the .ova file and click finish <br/>
<img src="https://i.postimg.cc/h4M5L9zs/Image-7.png" height="80%" width="80%" />
<br />
<br />

<p align="Center">
Once the file has been loaded you will see Qualys Virtual Scanner appliance as below:<br/>
<img src="https://i.postimg.cc/rF0NDWSK/Image-8.png" height="80%" width="80%" />
<br />
<br />

<p align="center">
Start the VM and you will see the screen below, enter the personalize this scanner code: <br/>
<img src="https://i.postimg.cc/tJVn43Lb/Image-9.png" height="80%" width="80%" />
<br />
<br />

<p align="Center">
You can find your personalization code inside your Qualys account as below  under appliances <br/>
<img src="https://i.postimg.cc/JnScxz81/Image-10.png" height="80%" width="80%" />
<br />
<br />

<p align="Center">
  Let the installation run
 <br/>
<img src="https://i.postimg.cc/6Qmd6pyd/Image-11.png" height="80%" width="80%" />
<br />
<br />

<p align="Center">
Once the installation complete, it will automatically assign an IP assigned from your home router internal IP <br/>
<img src="https://i.postimg.cc/dQd8vvvy/Image-12.png" height="80%" width="80%" />
<br />
<br />
<p align="center">
Go back to Qualys web page and click on "Add IPs for Scanning: <br/>
<img src="https://i.postimg.cc/fbp9nqrC/Image-13.png" height="80%" width="80%" />
<br />
<br />

<p align="Center">
Clicked New > Select IP Tracked Addresses <br/>
<img src="https://i.postimg.cc/bwdryHbB/Image-14.png" height="80%" width="80%" />
<br />
<br />

<p align="Center">
This will be the IP Address range that is given by your home router( in this case I will be using 192.168.0.x/24 IP address but keep in mind for free version Qualys only allow you to scan up to 19 IP address  <br/>
<img src="https://i.postimg.cc/mkbZ0QBV/Image-15.png" height="80%" width="80%" />
<br />
<br />

<p align="Center">Check the box and click add:
 <br/>
<img src="https://i.postimg.cc/d0rq3W04/Image-16.png" height="80%" width="80%" />
<br />
<br />
<p align="center">
Now go Back to Virtual Box and start the Windows 10 VM that we have set up previously : <br/>
<img src="https://i.postimg.cc/sDbdWpq8/Image-17.png" height="80%" width="80%" />
<br />
<br />



<p align="Center">
Moved the Outdated VLC and Firefox that had been downloaded previously into the VM and Install these 2 software <br/>
<img src="https://i.postimg.cc/6Q0mMRbB/Image-19.png" height="80%" width="80%" />
<br />
<br />

<p align="Center">
Set static IP for the VM <br/>
<img src="https://i.postimg.cc/44MF2XPH/Image-20.png" height="80%" width="80%" />
<br />
<br />
<p align="center">
Open Qualys web page and go to Option profiles > New  Option profile..: <br/>
<img src="https://i.postimg.cc/5yFpWFgY/Image-21.png" height="80%" width="80%" />
<br />
<br />

<p align="Center">
Name it as Basic scan and leave the other settings as default for now<br/>
<img src="https://i.postimg.cc/258sR2Z1/Image-22.png" height="80%" width="80%" />
<br />
<br />
<p align="Center">
Set the Netwwork adapter as Bridged adapter<br/>
<img src="https://i.postimg.cc/pLzM6LpG/Image.png" height="80%" width="80%" />
<br />
<br />

<p align="Center">
Turn off Firewall <br/>
<img src="https://i.postimg.cc/sDYqMtPB/Image-23.png" height="80%" width="80%" />
<br />
<br />

<p align="Center">
You should be able to ping from Host machine into guest machiine as below: <br/>
<img src="https://i.postimg.cc/66R1PDmH/Image-24.png" height="80%" width="80%" />
<br />
<br />

<p align="center">
Go back to Qulays web portal, go to scans click new scan: <br/>
<img src="https://i.postimg.cc/65czJwLh/Image-25.png" height="80%" width="80%" />
<br />
<br />

<p align="Center">
Set the scan name, scan profile, scan appliance name and IP address as below: <br/>
<img src="https://i.postimg.cc/LXjByM8L/Image-26.png" height="80%" width="80%" />
<br />
<br />

<p align="Center">
After that you will see the scan is now running and wait until it finishes <br/>
<img src="https://i.postimg.cc/B6f2PwB6/Image-27.png" height="80%" width="80%" />
<br />
<br />

<p align="Center">
You can view the scan result( keep in mind this is unauthenticated scan and thus it will only scan possible external vulnerabilities such as ports) <br/>
<img src="https://i.postimg.cc/T17y0kgn/Image-28.png" height="80%" width="80%" />
<br />
<br />
<p align="center">
Go to services.msc and set Remote registry to automatic and start the service: <br/>
<img src="https://i.postimg.cc/66jTDm4v/Image-29.png" height="80%" width="80%" />
<br />
<br />

<p align="Center">
Make sure the network discovery is turned on: <br/>
<img src="https://i.postimg.cc/8PfkxPV2/Image-30.png" height="80%" width="80%" />
<br />
<br />

<p align="Center">
Go to user acount control settings and set to never notify <br/>
<img src="https://i.postimg.cc/T1zxTgXZ/Image-31.png" height="80%" width="80%" />
<br />
<br />

<p align="Center">
Create registry as LocalAccountTokenFilterPolicy and set to 1 <br/>
<img src="https://i.postimg.cc/QxqD2Byn/Image-32.png" height="80%" width="80%" />
<br />
<br />

  Note: Keep in mind the following procedure is for demonstration process only, in a real world environment you want the authenticated scanning is performed by agent running on the machine.
  
<p align="center">
Go to Authentication -> Operating Systems -> Windows: <br/>
<img src="https://i.postimg.cc/jd1cdcmW/Image-33.png" height="80%" width="80%" />
<br />
<br />

<p align="Center">
Set the title <br/>
<img src="https://i.postimg.cc/Bv0xXVgv/Image-34.png" height="80%" width="80%" />
<br />
<br />

<p align="Center">
Set Windows local credentials and checked both authentication protocols <br/>
<img src="https://i.postimg.cc/rw64PP79/Image-35.png" height="80%" width="80%" />
<br />
<br />


<p align="center">
Input the IP Address of the machine that will be scanned: <br/>
<img src="https://i.postimg.cc/0Q3dndmM/Image-37.png" height="80%" width="80%" />
<br />
<br />

<p align="Center">
Go back to option profiles > edit:  <br/>
<img src="https://i.postimg.cc/vH5L7nmT/Image-38.png" height="80%" width="80%" />
<br />
<br />


<p align="Center">
Create new scan and filled them as below: <br/>
<img src="https://i.postimg.cc/bNRSN9Jx/Image-40.png" height="80%" width="80%" />
<br />
<br />

Note: I have encountered issue where the scan was not showing anything at all on the 2nd run and had to change the static IP address and restart the machine to resolve it.
You will see I changed it to 192.168.0.89 as per screenshot below.
<p align="center">
Compare to the unauthenticated scan now we can see more vulnerability showed up from our scans and now the severity is much higher : <br/>
<img src="https://i.postimg.cc/zDFGnXr5/Image-41.png" height="80%" width="80%" />
<br />
<br />

<p align="Center">
Every vulnerability has a risk score and rating and we can see the outdated application we have installed earlier also showed up in the scans result<br/>
<img src="https://i.postimg.cc/zGbNPq9y/Image-42.png" height="80%" width="80%" />
<br />
<br />

<p align="Center">
Once you click on it it will tell you what is the impact of the vulnerability and how to resolve it, so now we only need to investigate the CVE code and remediate the vulnerabilities based on the recommendations <br/>
<img src="https://i.postimg.cc/Gmy0xqyY/Image-43.png" height="80%" width="80%" />
<br />
<br />

<h2> End of Vulnerability Management Home Lab</h2>




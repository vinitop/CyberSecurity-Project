# RECON-Scripts
Scripts to automate RECON process


1) Subdomain enumeration with "Assetfinder" (by the genius of "Tomnomnom" https://github.com/tomnomnom/assetfinder) and Sublist3r (https://github.com/aboul3la/Sublist3r).

2) Sort to remove the duplicate entries (domains.txt)

3) Check assets alives with "HTTPROBE" (again... by Tomnomnom https://github.com/tomnomnom/httprobe)

4) Saved the alive domains in a different file called alive.txt.
Both outputs files (domains.txt and alive.txt also are in json format)

5) Create "headers" and "responsebody" directories

6) Looping through all the domains stored in alive.txt and sending cURL requests to fetch headers and response body and then storing them inside headers and responsebody directories

7) Collect all the JavaScript files from the response body text which we collected in the previous step

8) Using a tool called relative-url-extractor by Jobert Abma (https://github.com/jobertabma/relative-url-extractor) for  collect all the relative paths which are present in the JavaScript files.

9)At this point, the script will pass all the domains present in domains.txt to nmap and will store the result inside the nmapscans




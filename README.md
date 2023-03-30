# Bug-Bounty-Recon-Automation
This Python script automates the bug bounty recon process using various open-source tools for subdomain enumeration, directory scanning, port scanning, vulnerability scanning, and other techniques. Tools used include subfinder, dirsearch, nmap, vulners, and more. It saves time and improves efficiency
Bug Bounty Recon Automation
This is a Python script that automates the bug bounty recon process using various open-source tools. The script uses a combination of subdomain enumeration, directory scanning, port scanning, vulnerability scanning, and other techniques to help identify potential vulnerabilities in web applications.

Installation
To use this script, you must have the following tools installed on your system:

subfinder
dirsearch
nmap
vulners
GetJS
GoLinkFinder
getallurls
WayBackUrls
WayBackRobots
MassDNS
Sublist3r
FFuF
XSSHunter
SQLMap
XXEInjector
SSRFDetector
GitTools
gitallsecrets
RaceTheWeb
CORStest
EyeWitness
parameth
You can install these tools using your system's package manager (e.g., apt, yum, pacman) or by following the installation instructions provided by the tool's official website.
Usage
Clone this repository:
Copy code
git clone https://github.com/Plasmasecurity/Bug-Bounty-Recon-Automation.git
Navigate to the repository directory:
Copy code
cd Bug-Bounty-Recon-Automation
Modify the config.json file to specify your target domain and other options:

json
Copy code
{
  "domain": "example.com",
  "output_dir": "output",
  "tools": {
    "subdomain_enum": ["subfinder", "massdns", "sublist3r"],
    "dir_search": ["dirsearch", "ffuf"],
    "port_scan": ["nmap"],
    "vuln_scan": ["vulners", "sqlmap", "xxeinjector", "ssrfdetector"],
    "git_scan": ["golinkfinder", "gittools", "gitallsecrets"],
    "reconnaissance": ["getallurls", "waybackurls", "waybackrobots", "parameth", "eyewitness", "corstest", "racetheweb"],
    "javascript_enum": ["getjs", "subjs"]
  }
}
Run the script:

Copy code
python3 recon.py
This will run the script with the default configuration. You can modify the configuration by passing a different config.json file using the --config option:

css
Copy code
python3 recon.py --config /path/to/custom_config.json
The script will output the results to the output directory (or the directory specified in the output_dir field of the config.json file).

Contributing
Contributions and feedback are welcome and encouraged. Please create a new branch and submit a pull request for any changes or improvements you would like to make.

License
This code is licensed under the MIT License. See the LICENSE file for details.

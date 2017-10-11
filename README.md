# GeoIP2_Parser

# Introduction

Well come to GeoIP2 IP parser Automation Script Repo. This is a script that prints a list of test cases which can be found in projects root directory. 

Test cases are Written to validate Different IPv4 & IPV6 address by parsing them against standards rules. Description of the IP address format accepted by GeoIP2 web services can be found in this link.

At [GeoIP2 Precision Web Services/MaxMind Developer Site] (https://dev.maxmind.com/geoip/geoip2/web-services/), under the section IP Address, you will find a description of the IP address format accepted by GeoIP2 web services.


### Test Plan & Test Case 

This is a test automation scripts. that picks up a set off fault model IP address both for Ipv4 & Ipv6. 
Then it parse the IP address against standards rules - Validate them add a flag Ok(1) or Not Ok (0) with parsed IP and print it to command line in a Comma Separated value. 
example ( for full test case list see the testcase.txt file 
```
TestCase ID	|	IP	|	Type |	Description
======================================================================================= 	
Test 0		  |	me	|	IPv4	|	IPv4 address Min Boundary
Test 1		  |	0.0.0.0	|	IPv4	|	IPv4 address Min Boundary
Test 2		  |	27.0.0.1|	IPv4	|	IPv4 address Regular
Test 6		  |	2605:2700:0:3::4713:93e3	|	IPv6	|	public IPv6 address
```

Note: Don’t change the format of the test case in .txt file. it’s a BDD friendly test case can be used in Cucumber framework
       


### Prerequisites
This is a simple maven project created to make the script CI/CD ( continuous integration ) friendly. 
java & Maven need to be properly install on targeted nod to run this program. 

### Installing & Executing the Program 
simply clone the repo to any machine that has maven installed and run the [Run.sh] script. that’s it. 
for windows CD to repo folder and execute a ** mvn clean install command ** 

### Instruction 

while running in terminal it will ask for a Command line argument Q(Quick) or C (Comprehensive) 
q will print 5 record 
c will print 10 record 

Providing Wrong Input Will Loop through Until Right Input 
to force exit press Ctl + c 


## Authors

* **MD Rasul**

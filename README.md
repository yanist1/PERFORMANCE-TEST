
### PRE-REQUESITES

1. Register to get the API token key on this web 
```https://www.weatherbit.io/account/create```
2. Install Java and download Jmeter on this web
```https://jmeter.apache.org/download_jmeter.cgi```

### INSTALLATION
1. Clone the repository to your directory
   ```
   git clone https://github.com/auliabalqis16/performance-test-jmeter.git
   ```
3. Open {your directory}/apache-jmeter-5.5/bin
4. Open jmeter GUI
- use terminal and using following comand ./jmeter.sh (linux/mac os)
- double click jmeter.bat (windows)
5. change value`s token on 'User Defined Variables' to your API token

### HOW TO RUN
1. open terminal
2. go to {your directory}/apache-jmeter-5.5/bin
3. Enter following command, jmeter -n –t test.jmx -l testresults.jtl
-n: It specifies JMeter is to run in non-gui mode
-t: Name of JMX file that contains the Test Plan
-l: Name of JTL(JMeter text logs) file to log results
-j: Name of JMeter run log file

### HOW TO GENERATE HTML REPORT
1. go to {your directory}/apache-jmeter-5.5/bin
2. click Tools
3. click Generate HTML Report
4. input some item
 - Result file : JMeter run log file
 - user.properties.file (usualy in apache-jmeter-5.5/bin) 
 - output directory: empity folder directory
5. click generate html report
6. go to your output directory
7. there's html file report

### HOW TO TRIGGER CI
push something to master

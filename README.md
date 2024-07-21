# System-Configuration-Checker
Here's a shell script to verify and validate system configurations against predefined standards or configurations. This script will compare the current system configurations with a set of predefined standards stored in a configuration file. If there are any discrepancies, it will report them.

# Explanation:
PREDEFINED_CONFIG: The path to the file containing predefined configuration standards.
<br><br>
CURRENT_CONFIG: The path to the file where the current system configuration will be stored temporarily.
<br><br>
get_current_config: A function that collects the current system configurations. This example includes hostname, OS version, kernel version, firewall status, and SSH service status. You can expand this to include other configurations as needed.
<br><br>
compare_configs: A function that compares the current system configuration with the predefined standards using the diff command. If there are discrepancies, they will be printed out.
Main Script Execution: The script calls get_current_config to collect the current configuration and then compare_configs to validate it against the predefined standards.
<br><br>

# Summary
This script will help you ensure that your system configurations comply with predefined standards. You can schedule it using cron to run periodically and report any discrepancies automatically.

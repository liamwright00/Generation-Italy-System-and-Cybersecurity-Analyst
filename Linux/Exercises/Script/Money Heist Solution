#!/bin/bash

# Preparations for the Heist
mkdir -p /tmp/piano_colpo
echo "This is the plan for the heist." > /tmp/piano_colpo/strategia.txt

# Create a variable for the Professor's name
CAPOBANDA="Professor X"
echo "CAPOBANDA is set to: $CAPOBANDA"

# Device Preparation
cd /tmp/piano_colpo
touch dispositivo1.txt dispositivo2.txt dispositivo3.txt
ls dispositivo*.txt

touch equipaggiamentoA.log equipaggiamentoB.log equipaggiamentoC.log
ls *.log

# Add content to all 'dispositivo' files
echo "Resources updated" >> dispositivo1.txt
echo "Resources updated" >> dispositivo2.txt
echo "Resources updated" >> dispositivo3.txt

# Redirect output and error to log.txt
ls dispositivo* > log.txt 2>&1

# Security
ls -l strategia.txt
chmod 600 strategia.txt
ls -l strategia.txt
chmod 644 strategia.txt

# Heist Simulation
sleep 300 &
sleep_pid=$!
echo "Sleep process started with PID: $sleep_pid"

# Check running processes
ps -p $sleep_pid

# Suspend the sleep process
kill -SIGSTOP $sleep_pid
echo "Sleep process suspended."

# Terminate the sleep process
kill $sleep_pid
echo "Sleep process terminated."

# Generate high CPU load
yes > /dev/null &
high_load_pid=$!
echo "High load process started with PID: $high_load_pid"

# Monitor running processes
ps -p $high_load_pid

# Terminate the high CPU load process
kill $high_load_pid
echo "High load process terminated."

# Heist in Progress
MESSAGGIO="The heist is in progress."
echo $MESSAGGIO

# Create report.txt and log the current time
echo "$(date): Updated progress" > report.txt

# Create the status message script
echo -e "#!/bin/bash\necho 'Current status: Everything is going according to plan.'" > messaggio_stato.sh
chmod +x messaggio_stato.sh

# Execute the status message script
./messaggio_stato.sh

# Automating the Procedure
echo "Beginning the heist."
mkdir -p esecuzione
cp dispositivo* esecuzione/
chmod 600 esecuzione/*
echo "Heist completed."

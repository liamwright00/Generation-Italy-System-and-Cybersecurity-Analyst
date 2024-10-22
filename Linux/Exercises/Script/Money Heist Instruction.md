

### TODAY WE'RE GOING TO MAKE A HIT!

**Preparations for the Heist**
- Navigate to the directory `/tmp` and create a new directory called `piano_colpo`.
- Inside `piano_colpo`, create a file called `strategia.txt` and add a description of the heist plan (it can be a simple sentence).
- Create a variable called `CAPOBANDA` and assign it the value of the Professor's name.
- Print the value of the variable `CAPOBANDA` to confirm it is correctly set.

**Device Preparation**
- In the directory `piano_colpo`, create three files named `dispositivo1.txt`, `dispositivo2.txt`, and `dispositivo3.txt` that represent the devices needed for the heist.
- Using a single command, list all files that start with `dispositivo` and end with `.txt`.
- Create three more files called `equipaggiamentoA.log`, `equipaggiamentoB.log`, and `equipaggiamentoC.log`.
- Using a single command, list all files that end with `.log`.
- Add the content "Resources updated" to all files that start with `dispositivo` and end with `.txt`.
- Redirect the output and error of a command (e.g., `ls dispositivo*`) into a file called `log.txt`.

**Security**
- Check the permissions of the file `strategia.txt`.
- Change the permissions of `strategia.txt` so that only the Professor (owner) can read and write the file, while the group and others have no permissions.
- Check the permissions of `strategia.txt` again to ensure they are correct.
- Change the permissions of `strategia.txt` to allow the group and others to read it but not modify it.

**Heist Simulation**
- Execute a command that simulates a long operation (e.g., `sleep 300 &`).
- Check the running processes and locate the `sleep` process.
- Temporarily suspend the `sleep` process.
- Terminate the `sleep` process.
- Execute a command that generates high CPU load (e.g., `yes > /dev/null &`).
- Monitor the running processes.
- Terminate the process that generates high CPU load.

**Heist in Progress**
- Create a variable called `MESSAGGIO` with the value "The heist is in progress."
- Use the variable `MESSAGGIO` to print the message to the terminal.
- Create a file called `report.txt` in the `piano_colpo` directory.
- Use the `date` command to add the current time and the string "Updated progress" to the `report.txt` file.
- Create a bash script called `messaggio_stato.sh` that prints the message "Current status: Everything is going according to plan."
- Run the script to verify that it works correctly.

**Automating the Procedure**
- Write a bash script called `esegui_colpo.sh` that performs the following tasks:
  - Print the message "Beginning the heist."
  - Create a directory called `esecuzione` inside `piano_colpo`.
  - Copy all files starting with `dispositivo` into the `esecuzione` directory.
  - Change the permissions of all files in the `esecuzione` directory to make them readable and writable only by the owner.
  - Print the message "Heist completed."
- Run the script and verify that it works correctly.

--- 

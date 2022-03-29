- Using wireshark to read file capture.pcap. Export http object to receive:
      + 4A7xH.ps1
      + 9tVI0
      + user32.dll
- Using dnspy to reverse user32.dll and decrypt file 9tVI0 using Program.cs. base64 decode result to receive shellcode download.dat
- Using tool ShellcodeLoader.exe (https://github.com/sisoma2/ShellcodeLoader) to run shellcode:
      + cmd: ShellcodeLoader.exe  -a 1000 download.dat
      + using procmon64.exe of sysinternal to monitor to receive flag.

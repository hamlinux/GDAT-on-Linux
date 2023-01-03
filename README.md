# GDAT-on-Linux
My description of the steps to get the Genealogical DNA Analysis Tool (GDAT) working on Linux

- Download the ZIP file for your distributions architecture.
- Navigate to your Downloads directory.
- Extract the file using your preferred archiving tool into your PATH.
```bash
unzip 'Linux 64 bit.zip' /home/$USER/.local/bin
```
- Navigate to the binary.
```bash
cd Linux\ 64\ bit/Genealogical\ DNA\ Analysis\ Tool/
```
- Make the binary executable.
```bash
chmod +x Genealogical\ DNA\ Analysis\ Tool/
```
- Create a Softlink to easily run the executable from the terminal.
```bash
ln -s /home/$USER/.local/bin/Linux\ 64\ bit/Genealogical\ DNA\ Analysis\ Tool/Genealogical\ DNA\ Analysis\ Tool /home/$USER/.local/bin/gdat
```
- Run from the terminal and detached if the link is located within $PATH.
```bash
gdat &
```

- Simply changing the name of the binary will result in an error.
- Tested on Debian 11.3 Stable requiring no additional dependencies.

Remote update of esp32 board in esphome via http request.

Http update useful when the esp32 board is not in the same local network as the HA server.

The .ota.bin file should be generated in esphome.

Then you should create .md5 file in PowerShell and upload to the server, e.g. your github project.

In the created software button on esp run updates from http.


#########################################

Windows PowerShell

command to FilePath pv-offgrid.md5 :

(Get-FileHash -Path pv-offgrid.ota.bin -Algorithm md5).Hash.ToLower() | Out-File -FilePath pv-offgrid.md5 -Encoding ASCII

command to FilePath dc-ac-offgrid.md5 :

(Get-FileHash -Path dc-ac-offgrid.ota.bin -Algorithm md5).Hash.ToLower() | Out-File -FilePath dc-ac-offgrid.md5 -Encoding ASCII

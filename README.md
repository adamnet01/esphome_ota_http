https://github.com/adamnet01/esphome_offgrid

Windows PowerShell

command to FilePath pv-offgrid.md5 :

(Get-FileHash -Path pv-offgrid.ota.bin -Algorithm md5).Hash.ToLower() | Out-File -FilePath pv-offgrid.md5 -Encoding ASCII

command to FilePath dc-ac-offgrid.md5 :

(Get-FileHash -Path dc-ac-offgrid.ota.bin -Algorithm md5).Hash.ToLower() | Out-File -FilePath dc-ac-offgrid.md5 -Encoding ASCI

HOW TO REJOIN THE APK FILE
==========================

The file "tsis-prod-v2.3.8-202401261146.apk" was split into 6 parts
(.001 through .006) so each fits under a 25 MB email attachment limit.

Put all 6 parts in the SAME folder, then rejoin them in order.

--------------------------------------------------
WINDOWS (Command Prompt / cmd)
--------------------------------------------------
Open cmd in the folder with the parts and run:

    copy /b tsis-prod-v2.3.8-202401261146.apk.001 + tsis-prod-v2.3.8-202401261146.apk.002 + tsis-prod-v2.3.8-202401261146.apk.003 + tsis-prod-v2.3.8-202401261146.apk.004 + tsis-prod-v2.3.8-202401261146.apk.005 + tsis-prod-v2.3.8-202401261146.apk.006 tsis-prod-v2.3.8-202401261146.apk

--------------------------------------------------
WINDOWS (PowerShell)
--------------------------------------------------
    cmd /c "copy /b tsis-prod-v2.3.8-202401261146.apk.001+tsis-prod-v2.3.8-202401261146.apk.002+tsis-prod-v2.3.8-202401261146.apk.003+tsis-prod-v2.3.8-202401261146.apk.004+tsis-prod-v2.3.8-202401261146.apk.005+tsis-prod-v2.3.8-202401261146.apk.006 tsis-prod-v2.3.8-202401261146.apk"

--------------------------------------------------
MAC / LINUX (Terminal)
--------------------------------------------------
    cat tsis-prod-v2.3.8-202401261146.apk.0* > tsis-prod-v2.3.8-202401261146.apk

--------------------------------------------------
VERIFY THE RESULT (optional but recommended)
--------------------------------------------------
The rejoined file should match this SHA256 checksum:

    C74533627DB361917545817827C5CC2E515B95E4B60E9B892D9488965E1655D3

Windows PowerShell:
    Get-FileHash tsis-prod-v2.3.8-202401261146.apk -Algorithm SHA256

Mac:
    shasum -a 256 tsis-prod-v2.3.8-202401261146.apk

Linux:
    sha256sum tsis-prod-v2.3.8-202401261146.apk

If the checksum matches, the file rejoined correctly and is ready to install.

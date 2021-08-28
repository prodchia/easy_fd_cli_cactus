# easy_fd_cli_cactus

Easy windows version to install and run https://github.com/Cactus-Network/fd-cli

[1] git clone https://github.com/prodchia/easy_fd_cli_cactus.git

[2] cd easy_fd_cli_cactus

[3] easy_setup.bat

[4] Open config.cfg and complete the required information there

Wallet fingerprint found at below path or by using "chia wallet show"

Launcher ID: can be obtained using "chia plotnft show"

Pool contract address: can be obtained using "chia plotnft show" and it should start with xch

Window User is the windows user name under which you are currently working.

That's it.

Now to recover coins:

[5] get_coins.bat coinname(e.g. cactus)


This version works with forks like cactus that are based on the latest chia code( >1.2.0). To recover from blockchains based on the legacy chia code use the easy_fd_cli version.(https://github.com/prodchia/easy_fd_cli)


There are some slight differenes between various blockchains. To recover  coins  other than cactus use the easy_fd_cli version ( https://github.com/prodchia/easy_fd_cli)

If you receive the error "ImportError: DLL load failed while importing blspy: The specified module could not be found", it's likely due to the missing Visual C++ redistributable package used by blspy. You can try to the reinstall blspy.

[a] Go to the easy_fd_cli directory

[b] call .\venv\Scripts\activate

[c] pip install blspy

If [c] works try to run get_coins.bat. If it doesn't then it probably crashed with some error like c++ not found. You can download and install what it is asking for, and follow the steps from a-c. Hopefully it should work

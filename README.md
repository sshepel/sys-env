### MS Visual Studio Code

Get list of plugins:

	code --list-extensions --show-versions > msvsc/msvsc-extensions.txt

Import plugins:
	cat msvsc/msvsc-extensions.txt | xargs -L 1 echo code --install-extension

	type msvsc/msvsc-extensions.txt | % { &code --install-extension $_ }

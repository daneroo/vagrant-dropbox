# Dropbox on a headless linux

See [this link](https://www.dropbox.com/install?os=lnx)

	vagrant up
	vagrant ssh
	# creates ~/.dropbox-dist/
	cd ~ && wget -O - "https://www.dropbox.com/download?plat=lnx.x86_64" | tar xzf -

	# now run the daemon
	~/.dropbox-dist/dropboxd

Which produces this, (after we visit the link)

	Please visit https://www.dropbox.com/cli_link?host_id=02966eaa113ea1db180696c14c36787c to link this machine.
	Please visit https://www.dropbox.com/cli_link?host_id=xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx to link this machine.
	Client successfully linked, Welcome Daniel!

See [this link](http://nixgeek.com/headless-dropbox.html) to make a service:
*Rails Blog Application*

[Ubuntu Setup]
SMBus base address uninitialized - upgrade bios or use force_addr=0xaddr

1. Check module is being loaded
$ lsmod | grep i2c_piix4
2. If so, blacklist it in the file /etc/modprobe.d/blacklist.conf, by adding the following to the end of the file:
+ blacklist i2c_piix4
3. Update the initramfs
$ sudo update-initramfs -u -k all

$ rails -T . 
$ git init
$ git add . 
$ git commit -m "Initial Commit"
$ git remote show origin 
$ git remote set-url origin git+ssh://git@github.com/username/reponame.git

[app/models/moderator.rb]
+ has_secure_password

[db/seeds.rb]

+ moderator = Moderator.create(
	fullname: "Daniel Park",
	username: "menoelpis@gmail.com",
	password: "shema")

$ rake db:seed
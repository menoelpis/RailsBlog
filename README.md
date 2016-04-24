*Rails Blog Application*

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
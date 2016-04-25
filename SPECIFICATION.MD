Moderators

	Actors
		-moderator
			# Create
				* is created the first time app is seeded
			# Read
				* visiting index page, should show the moderator's record
				* can see edit link whilst viewing moderator
				* cannot see delete link whilst viewing moderator
			# Update
				* can edit own moderator profile
				* show success/failure flash message
			# Delete
				* moderator cannot delete themselves

Sessions

	Actors
		-moderator
			# Visit any admin pages
				* pages should all be behind an authentication system
				* you should require username and password to login
				*ability to logout by clicking logout link
			# Create
				* ability to create a new login session for a moderator
					> by filling in username and password
					> session should remember
			# Read
				* logout link on all pages that calls session destroy
			# Delete
				* destroy session
				* show success/failure flash messages
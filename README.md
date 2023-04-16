DEVELOPED by SOHAM K CHATTOPADHYAY

Soft skills refer to a person's interpersonal abilities, such as communication, teamwork, problem-solving, adaptability, time management, leadership, and emotional intelligence.
This puzzle is designed to to measure a person problem solving ability and also their time management ability. The given puzzle is similar to a question in competative programming which is an essential factor in a programmers life when it comes to interviews or even hobbies.

#####################################

The possible ways to solve the puzzle include submission of a code strictly developed in python for the application to evaluate it and also proceed to the next level of the puzzle
It consists of my room(the actual puzzle) and an example room which can be considered as a demo or even as a test case.
My room consists of 2 levels and each level consists of 2 codes to help the user analyze and come up with a practical and feasible solution to the problem
Also, new rooms can be created locally depending upon the users requirements. The method to do the same is mentioned below

####################################

HOW TO RUN:

Just start EscapeRoomWeb.py or use the batch file start.bat (on Windows). This will start a web server on http://localhost:5000. Please open this URL in your web browser to start the game.

HOW TO CREATE A SOLUTION:

As a player you will have to develop little algorithms in Python with your favorite editor (which you store locally) to solve the challenges. For every level you have to create a .py-file with a method called run and one parameter.
	def run(secret):
	pass

HOW TO CREATE A NEW ROOM:

As a developer you may want to create new rooms and levels. All rooms are Python classes in the 'rooms' folder. They should be derived from class EscapeRoom:
	class AnotherRoom(EscapeRoom):

And they must have an init method with the following code:

def __init__(self):
		super().__init__()
		self.set_metadata("Your name", __name__)
		self.add_level(self.create_level1())
		self.add_level(self.create_level2())
		# add more levels like above


FEATURES IMPLEMETED IN THE WEBAPP:
1) The puzzle has clues and can assist the user when needed
2) Flask is used with python to set up the environment for working
3) Consists of a feature of creating additional rooms where the user is able to design neww puzzle and supply clues according to his convinience. This is mainly a suitable function for admins to work upon for users.
4) Automated test cases include an example room which is present in the menu to understand the functioning of the program.



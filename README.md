Slack AgeBot – Instant Age Calculator  
A simple Slack bot built using Golang and Slacker that calculates a user's age based on their year of birth (YOB).  

🚀 Features  
✅ Calculates age based on the provided year of birth  
✅ Interactive Slack commands for seamless user experience  
✅ Uses Slacker for easy Slack bot integration  
✅ Logs command events for debugging and analytics  
✅ Lightweight and efficient Golang-based bot  

🛠️ Technologies Used  
🐹 Golang – Backend programming language  
🤖 Slacker – Slack bot framework  
🔗 Slack API – Integration with Slack  
⏳ Time Package – For age calculation  
📝 Logging – Captures command events  

📥 Installation & Setup  

Installation & Setup:

Clone the Repository
git clone https://github.com/your-username/slack-age-bot.git  
cd slack-age-bot  

Install Dependencies
Ensure Golang is installed, then run:
go mod tidy

Configure Environment Variables
Set your Slack bot credentials in the environment variables:
export SLACK_BOT_TOKEN="your-slack-bot-token"  
export SLACK_APP_TOKEN="your-slack-app-token"  

Alternatively, update them in the main.go file using:
os.Setenv("SLACK_BOT_TOKEN", "your-slack-bot-token")  
os.Setenv("SLACK_APP_TOKEN", "your-slack-app-token")  

Run the Application
go run main.go  

The bot will start listening for commands in Slack.

Usage:
Once the bot is running, use the following command in Slack:
my yob is <year>  
Example:
my yob is 1996  
The bot will respond with your age:
Your age is 29.

Project Structure:

python
Copy
Edit
slack-age-bot/  
│── main.go             # Entry point for the bot  
│── go.mod              # Go module file  
│── go.sum              # Dependency tracking  
│── README.md           # Documentation 

Deployment:
You can deploy the bot using Docker or a cloud service.

Docker Deployment:
docker build -t slack-age-bot .  
docker run -e SLACK_BOT_TOKEN="your-token" -e SLACK_APP_TOKEN="your-app-token" slack-age-bot  

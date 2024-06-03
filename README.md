<p align="center"><img src="https://github.com/thecoder-001/MineColab/blob/master/Logo.png" alt="Logo" height="80"/></p>
<h1 align="center">700's MineColabs</h1>
 <p align="center">
   <img src="https://img.shields.io/badge/STATUS-IN%20DEVELOPMENT-green">
   <img src="https://img.shields.io/github/stars/prozoon700?style=social">
</p>
<p align="center">
This is a modificated version of MineColab (original by: <a href="https://github.com/thecoder-001/MineColab">thecoder-001</a>), optimized, prepared for Forge and "with a UI".
This version is created by Prozoon700 and originaly made in Spanish!
</p>
<h4 align="center">
:construction: Project in development, if you find some issue or have any suggestion please add it to the <a href="https://github.com/Prozoon700/700s-MineColabs/issues">issues area</a>
</h4>

<br>

## :hear_no_evil:  First of all, what is google Colab?
As the official FAQ says, colaboratory, or “Colab” for short, is a product from Google Research. Colab allows anybody to write and execute arbitrary python code through the browser, and is especially well suited to machine learning, data analysis and education. More technically, Colab is a hosted Jupyter notebook service that requires no setup to use, while providing free access to computing resources including GPUs.
In short, it is a vm provided for learning, running python code, machine learning or for general purpose.
## :moneybag:  Is it really free to use?
Yes, Colab is free to use. But there are some points which, according to me one should keep in mind:
1. Though colab is a free service, it shouldn't be exploited indiscriminately or without any care. One should value that its a resource offered for no cost and can get depleted/restricted if the demand increases out of control.
2. If it isn't obvious, one shouldn't run mission-critical services (like large and important servers/databases/python programs) on it. Its resources are not guaranteed and not unlimited, and the usage limits sometimes fluctuate. Also, the notebook has a maximum runtime of 12 hours, after which, it should be manually restarted.
3. If you need to use it pretty often for intensive tasks, consider purchasing a vps server. A heavy increase in server load would force google to close the service.

In the end, it is just my personal opinion and can be ignored safely. Just ask your heart whats right and whats wrong. Also, please try to use it as a once in a while resource and not 24x7 so that others can avail the free resources too.

# :hammer: Characteristics
 - **Forge Compatibility:** MineColab is now compatible with almost any version of Forge.
   - *What does it mean?* You can now include mods on your servers. Important: Produces Lag and Ping of 1 to 4 seconds of delay in response time.
   - Tested with Minecraft versions: 1.12.2, 1.18.2, 1.20.1, 1.20.2
   - Tested with Forge versions: 14.23.5.2859, 40.2.0, 47.2.0, 48.1.0

 - **Performance improvement:** After a long time of development and searching, I have optimized the server with Java Flags, improving performance considerably.
   - *What does it mean?* Now the server works better, it usually does not have lag or delay in response (Playing with Paper).

 - **Creation of a UI:** I have created a "User Interface" so that the creation and in general all the steps are simpler and more visual for the creators.
   - *What does it mean?* Now instead of modifying code, you will simply add values ​​to some fields that are seen visually.

 - **Expanded customization:** You can now customize secondary things like folder names and regions.
   - *What does it mean?* Now you can have everything "more organized" and configured to your liking.

# :page_with_curl: Instructions
1. First execute the "Creating the necessary files" introducing the data you are going to use (Server Type, Minecraft Version, Forge Version (in case you use Forge) and the Directory Name, where the server files will be saved.), checking first that all is correct.
   <br>
   - Server Type -> Introduce the software you want the server to run.
     - Vanilla (no mods, but plugins) is "Paper".
     - Forge (no plugins, but forge mods) is "Forge".
     - Fabric (no plugins, but fabric mods) is "Fabric"
     - More software will be added as soon as possible!
   - Version -> Here you'll need to put the Minecraft version your server is going to use.
   <br>
   <br>
2. Then run again the cell (Creating the necessary files) and this time it should take longer, because all the files are being created and mounted.
   <br>
   <br>
3. Now you'll need to add a secret to the Colab Notebook (Project), for this go to the left side menu and click the key icon.
   - Add a new secret with the following data:
     - Name: server_directory
     - Value: `Shown in the terminal`
   - Check that the notebook (project) has access to the secret by turning on the switch.
5. Now that your files have being created you can check them going to the bottom (Visualize the folder files) and running the cell or checking the visualizer boolean input.
   <br>
   <br>
6. After this, go to the top until the "Starting the server" topic and fill the inputs with the necessary data.
   - OpenJDK (Java) version -> Enter the OpenJDK (Java) version you'll need to run your server.
     - If you don't know what OpenJDK version you need to use go to the topic "What OpenJDK version do I need?" and enter your Minecraft version following the steps on the input description.
   - Agent service -> This input is where you need to decide which agent are you using. Each agent has its own benefits and disadvantages.
     <br>
     | Agent Name  | Billing | Link | Pros | Cons |
     | ------------- | ------------- | ------------- | ------------- | ------------- |
     | `Ngrok`  | Partialy Free | [Web](https://ngrok.com)  | - Free region change. <br> - Better conectivity and timing.  | - Limited data transference of 1 GB. <br> - Delay of data transference renovation of 1 mo. |
     | `PlayIt`  | Free | [Web](https://playit.gg)  | - Unlimited data transference. <br> - Simple dashboard connection. | - Global region, premium to change. <br> - Worst connectivity and timing in some cases.  |
     | `Cloudflared` | Free and paid | [GitHub](https://github.com/cloudflare/cloudflared) | - Unlimited data transference. <br> - Multiple sub-domains. | - Difficult to install. <br> - You need a domain. |
     
      *Billing topic ensures that you can play mostly good without paying anything.
   - Region -> Only necessary when using ngrok agent.
   - PlayitMessages (1,2,3) -> Only necessary when using PlayIt and want to delete the custom messages PlayIt spams on the console.
   <br>
7. When all the needed inputs are filled run the cell (Starting the server) and if all the steps were correctly followed the server should start.
   <br>
   <br>
8. To stop your server first try running the stop command on the terminal.
   -  If the server restarts (after confirming that the worlds and data are saved) you can force stop the server by stopping the cell execution.

# :question: FAQ
- The server does not start.
  - Check if the files have been created.
    - If only the server.jar file has been created re-run the cell "Creating the server files".
    - If any file has been created check that the software and the versions are correctly spelled and they exist on Paper, Forge, Fabric, etc... web page.
    - If all the files have been created but the server does not start continue reading.
  - Check that the config in the "Starting the server" cell is correct and not misspelled.
    - If something is wrong, stop the server if it's running, change the value, save the data and re-run the server.
    - If everything is correct, check that the Java version is correct.
    - If all the configs are good and the Java version is the correct one check the terminal for error and paste them on the [Issue Page](https://github.com/Prozoon700/700s-MineColabs/issues).
 - Check that Google Colab has the permisson to acces Google Drive.
   - If not it should be requested, grant the permission to Google Drive if you want the server to work.
   - If it has permission check the terminal for error and paste them on the [Issue Page](https://github.com/Prozoon700/700s-MineColabs/issues).
- The server files are not created
  - Check the config input values
    - If there is something wrong, stop the cell by clicking on the square button at the left side of the cell, modify what you need and re-run the cell.
    - If everything is okey continue reading.
  - Check that the server's directory is on a secret with the correct name and value.
    - If not, change the name / value and try again.
    - If it's correct continue reading.
  - Check that Google Colab has the permisson to acces Google Drive.
   - If not it should be requested, grant the permission to Google Drive if you want the server to work.
   - If it has permission check the terminal for error and paste them on the [Issue Page](https://github.com/Prozoon700/700s-MineColabs/issues).
- How do I make my own a server operator?
  - Write in the terminal the following command: `op {your-nametag}`
- How much time will my server stay on?
  - Commonly a server can be at a maximum of 12 hours after being stopped if any external feature it's acting on the server's start up time.
  - You can check this by following this steps:
  - `Top Menu` > `Runtime Environment` > `See Resources` > `Below the title menu or the resources graph`
# :crystal_ball: The Project's Future
- I would firstly like to have some guys that want to test out the beta versions so I can easily found bugs and solve them (and I'm also capable of touching grass🌿).
- The project should and must be continued, so I'll do my best to update it and solve the bugs that you and I find out.
- I'll try to make a real User Interface (web) when you can control and manage things a lot much easier. It will be based on Pterodactyl's Panel.

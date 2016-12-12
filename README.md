# How to use Github #
<i>Made by Marco van de Lindt en Daan de Vos</i>
<br />
<h3>Nowadays almost every programmer uses, or at least knows, GitHub. GitHub is a webiste which makes it super simple for you to start projects, share projects with the rest of the world, and work together. Since we're using GitHub too, we took the time to make a tutorial for you, just to understand the basics of GitHub.</h3>
<p>First of all, let's open GitHub in our Browser. I highly doubt you haven't opened it already, since you're reading this tutorial right now.</p>
<hr />
# Setting up your account #
<p>When you're not signed up for an account already, you can do that right know. Registering an account for GitHub is super easy, so let's do that right now. First, we pick our username. Choose something that's easy to remember, but also something you like. After that, you fill in you're email address. Use your real email address, because you have to verify your account after you registered! At last, let's choose a password. Use something that's easy for you to remember, but not too simple. </p>

<p>After you've signed up, you're redirected to a screen where you can choose what kind of account you would like. You can just use a free account, but if you're planning on using a lot of private repositories, the best choice for you will be the 7 dollar a month plan. After this, let's press the continue button.</p>

<p>On this screen, you can customize you're account. This is al up to you. Just fill in how experienced you are, what you're planning on using GitHub for, describe yourself and choose subjects that you're interested in. After you've filled everything in, let's hit that submit button!</p>

# Start a project #
<p>Now, we can really start using GitHub. If you want more information about GitHub, feel free to read the guide. Otherwise, let's start a new project.</p>

<p>If you haven't verified your email address already, make sure to check your inbox and verify it. Otherwise you won't be able to start a new project. If you've filled in your email correctly, on top of you're inbox an email from GitHub has appeared. Open it and click on the link to verify your email address. Now, you'e able to start you're own new project!</p>

<p>First of all, let's give our repository a name. Since we're doing this with a tutorial, we'll call this <i>'Tutorial'</i>. After that, you can give your repository a description. Fill in the details of you're project. If you don't want to write a description, just leave the field blank.</p>

<p>Then, you can choose whether you make your repository private or public. For now, it doesn't really matter. If you don't want anyone to see your project, just click the <i>'Private'</i> one. Otherwise, you can just leave it on <i>'Public'</i>.

<p>At last, you can choose to initialize your repository with a README.md file. In this file you write certain information about your project, which can be of importance for the users who see or use your project. For now, we just initialize the repository with a README.md file.</p>

<p>Right in front of you, you're repository is visible. But how are we going to use this. GitHub has an online editor to write your code, but you can also clone everything to your own computer to work from there. We'll give you information on both ways.</p>
<hr />

# Setting up Git #

<p>To use Git, you have to download it. This is not very hard, just copy this link in your browser: https://git-scm.com/downloads.</p>

<p>On this page you can choose you're operating system. We are using Windows at the moment, so we click the <i>'Windows'</i> link. If you're using an other Operating System, just clik the right link for it. After that, you're download automatically starts. The download time depends on the speed of you're internet connection, but it shouldn't take too long.</p>

<p>After your download has finished, accept it when you've clicked your download.The following screen that pops-up, is just something you fill in yourself. For now, we just leave it as it is. Important is to use Git from the Command Prompt, that makes your life so much easier. The next screen is something you can choose for yourself again, we just leave it with the default settings. Just do this on the following pages, and your Git will start installing on your computer. This can take a littlw while, don't worry. After your download has completed, just click the finish button. No need to open GitBash.</p>

<p>If now errors occur, congratulations. You have now successfully set up Git. Now we can clone our projects to certain folders and so on. Let's dive right in to it!</p>

<hr />

<h3>Clone the repository to your computer</h3>

<p>Remember the repository we made at the beginning of this tutorial? Now, we can clone it to our computer and use our own Text Editor or IDE to write code. This is really simple, you just have to know the right commands. Don't worry, we'll help you with that!</p>

<p>When you look to the right of your screen, you can see the green: <i>'Clone or Download'</i> button. A link will then appear, with the repository we just made. Just press Ctr-C, or however you like to copy text.</p>

<p>The next thing is choosing the right folder to clone our repostory to. Since I'm using XAMPP, in the htdocs folder I create a new foler called <i>'Git'</i>. Now, open the <i>'Git'</i> folder, hold shift and right click in the folder. A menu now pops up. If you've hold the shift button, now a link with <i>'Open command prompt here'</i> will appear. Click on this and your command prompt will open. </p>

<p>Now, we're going to use our first command. You can't just paste the link you copied earlier, because nothing will happen. When you want to clone your repository, you obviously have to use the <i>'Clone'</i> commmand to do this. Remember that before all your command, you have to use to word <i>git</i>, otherwise it won't work. Now just type in: <i>git clone</i> and the paste the link you copied earlier. After that, hit enter and your repository will be cloned.</p>

<p>If no errors occur, you're repository has been successfully cloned. Inside the <i>Git</i> folder, now your repository is visible. Shut down your command prompt for now and open the created folder. Inside this folder, open your command prompt again. If you leave your command prompt open in the Git folder, Git wil not recognize the repository as a <b>Git</b> repository. Now we can start the real deal!</p>

<hr />

# Using Git #

<p>First of all, let's create a new file called index.php, or something else you like, and save it in the folder. When you return to your command prompt and type in the following command: <i>git status</i>, you'll see that with red letters the recently made file is visible. We want this file to be displayed at our GitHub page to, so we just do the following:</p>
<ul>
<li>We use the <i>git add *</i> command. The star means that we're adding everything, but for now it's only the index.php file. If in further projects you've worked on more file, but you ony want to add one file, just use <i>'git add index.php'</i> for example, and only the selected folder will be added.</li>
<hr />
<li>After you've hit enter after the <i>git add *</i> command, we've successfully added the index.php file. But if you look on your GitHub page, no index.php file is visible. This is because we have not send the actual file to GitHub. This is done with the <i>'git push'</i> command. What we have to do, before we push the index.php file to your GitHub page, we have to give a short description with it. This is done with the <i>git commit -m ""</i> command. Between the double quotes, you fill in the short description of what you just did. In this case we just type this: <i>git commit -m "added the index.php file"</i>. After we hit enter, you've successfully commited your file.</li>
<hr />
<li>Now, it's time to push your file to your GitHub page. This is done with the following command: <i>git push</i>. Just type in the command, and if no errors occur, you've successfully pushed your first file to your GitHub page.</li>
<hr />
</ul>
<p>Now, the only thing you have to do is just refresh your browser, or webpage. A new file has appeared in the list, called index.php. Congratulations! You've successfully used Git and uploaded your first file. From now on, you can do this with all the files you add or edit.</p>

<hr />

# Adding files from the GitHub page #
<p>If you don't want to use a text-editor, you can choose to work directly from your GitHub page. On the left side of the green <i>Clone or download</i> button, you can see a button called <i>Create file</i> Click on the button and you'll be redirected to a page where you can add your file and write yout own code. Pretty easy isn't it? </p>

<p>Just above your text field, you have to give your file a name. Just use an name you want to give it, and choose the right extension. If you only want to use <b>HTML</b>-code, you give your file the .html extension. If you want to use <b>PHP</b>-code in your file, you give it the .php extension. This goes for all the programming languages you wan't to use.</p>

<p>After you named your file and chose the right extension, you can start writing your code. In here you can write everything you like. Don't worry too much about what you're writing, you can always edit it later on.</p>

<p>After you wrote your code, you can save it to yout GitHub page. Simply scroll down to the end of the editor, and you'll se the section with: <b>Commit new file</b>. In the fist field, you almost do exactly the same as we did in the command-prompt. The only thing that's different, is that you don't have to use any command. Just simply write down what you just did, and you're good to go. You can add some additional info to, but that's not neccasary. When you've filled in al the information you wanted to give it, just click the <i>Commit new file</i> button. Now, you're redirected back to your repository page, and your commited file will be visible. When you click on it, you can see the code you just wrote. Isn't that awesome?</p>

<hr />

<h3>Editing your code</h3>

<p>When you click on your code, you notice that you can't edit anything. When you look at the right of your screen, you'll see a section with buttons. If you click on the pencil-icon, you are able to edit your code. After that, just commit the new changes you've made, and your edited file will be saved and updated with the code you just wrote.</p>

<hr />

# Adding Folders #

<p>Maybe, you've already know that there isn't a button for adding folders. In GitHub you can't officially add folders, but there is a small workaround, which will create a folder for you. Only thing you have to keep in mind, is that you always need a file in your folder, otherwise the folder won't be noticed by GitHub.</p>

<p>Adding folders through GitHub is pretty simple. Just click on the <i>Create new file</i> button. Instead of naming your new file, we create a folder just by giving it no extension. If you type in: <i>Test/</i>, you'll see that automatically, a new input field is added. In this field you can add a new file, or more folders if you want. Just make sure you always end with a file in the last folder. Now, when you go back to your repository, you'll see that the Test folder is added, and the file is inside that folder. That wasn't too hard wasn't it?</p>

<hr />

# Adding folders through the command prompt #

<p>There isn't a command, which just allows you to add folders to your repository, just like there isn't a command to make files. This has to be done by hand, but that's pretty simple.</p>

<p>In your project, just create a new folder and call it whatever you like. When you then go to your command prompt and use: <i>git status</i>, you'll see that it doesn't see the new folder you've just created. However, when you add a file to that folder and type <i>git status</i> again, you'll see that git has noticed that there's a new file available. From now on, you just do the same thing as adding a new file. Just use <i>git add</i>, to add your file. The use <i>git commit -m ""</i> to commit the changes you made and at last you use <i>git push</i>, to push it to your GitHub page. When you refresh the page, a new folder has appearedwith the file whitin it.</p>

<hr />

# Pull files made on the GitHub page, to your folder #

<p>We've already came to the end of the tutorial. But there's still something that's pretty convenient to know. If you ever add a file to the GitHub page, or you're working in a team and other people made new files, you have to pull those files to your folder. This is really simple. You just use the <i>git pull</i> command, and the added files are added to your folder</p>

<hr />

# Change the settings of your repository #

<p>It can always happen that when you progress in a project, you want to change some settings to in repository. This is really simple. Below your accountname there is a menu, with different links. When you go to the last link, you'll see <i>Settings</i>. When you click on this link, you can edit the settings of your repository.</p>

<p>If you want to change the name of your rpository, you can do that in the first text-field. Below that, you can turn on or turn off some features. Below that section you can edit your merges. In this tutorial, we are not going to discuss that, since this is just a tutorial of the basics of GitHub. At the very bottom of the page, you have the so called <i><b>Danger Zone</b></i>. Here, you can make your repository puclic of private, depending on which of one the two your repository is right now. You can transfer your ownership to someone else and at last you can delete your repository. Since those changes can be pretty big, GitHub always asks for a confirmation when you want to change those settings.</p>

<p>At the top of the page, on the left side, you also see a side-navigation. To check out what you can edit there, you have to figure that out yourself right now. 

<hr />

# Edit your profile #

<p>Ofcourse, you can always edit your profile. You can upload a profile picture, change / add information about yourself and much more.
Let's add a few details to our account!</p>

<p>On the right top of your screen, you can see your current profile picture. When you click on that picture, a dropdown menu will appear. When you click on <i>Your profile</i>, you will be redirect to a page where you can see your profile. On the left side of the screen, you can see your profile picture, but this time a lot bigger. Below that picture, you can see the button with <i>Edit profile</i>. Click on this button and you can added your profile</p>

<p>On this page you can add or change the following things:
<ul>
<li>Name</li>
<li>Email Address</li>
<li>Bio</li>
<li>Add a URL to your website for example</li>
<li>Company</li>
<li>Location</li>
</ul>

<p>Once you've finished editing or adding everything you would like, you just click on the <i>Update profile</i> button. From heren on, you can check out all the other things that you can change whithin your personal settings.</p>

# Creating new Repositories #

<p>In the future, you are likely going to start more projects whithin GitHub. To add a new Repository, you just click on the <b>+</b> syymbol, next to your profile image. Another dropdown menu will appear and you simply click on the <i>New repository</i> link. From here on everything we've learned in this tutorial will repeat. Now, try and set up your own repository, it isn't that hard!</p>

# Our final words #

<p>Hopefully, you've learned the basics of GitHub and using Git after reading this tutorial. From now on, you can expand your knowledge and learn more and more about GitHub. Thank you for reading this tutorial, and if it helped you, we're really glad.</p>

<b>Greetings, </b>

<i>Marco van de Lindt & Daan de Vos</i>

<style>
  h1{
    color:blue;
  }
  
 </style>

<h1>Installing git</h1>

<ul>
  <li>Follow these instructions: <a href = "https://git-scm.com/book/en/v2/Getting-Started-Installing-Git">git installation (Mac, Linux)</a></li>
  <li>Windows installation: <a href="https://support.codebasehq.com/articles/getting-started/git-on-windows">git installation(Windows)</a></li>
  <li>Verify installation by typing the following command in your terminal<strong>(MAC / Linux)</strong> or command prompt<strong>(Windows)</strong>:</li>
  <ul>
    <li><strong>Command:</strong><em> git --version</em></li>
  </ul>
  
 </ul>

<h2>Using git</h2>
<p>If you followed the instructions on installing git on Mac, Linux, or Windows, then all the code below will work regardless of the OS.  The code is based on bash commands, which are native to UNIX environments.  The windows installation guided you through the process of installing git in a way that you can use bash commands.</p>


<h2>Command list</h2>
<p>The following are commands that are commonly used for reference:</p>
<ul>
  <li><strong>git init</strong> -> will create a new repository in the directory(we wont need to use this)</li>
  <li><strong>git clone "repository url"</strong> -> clones an existing repository into current working directory</li>
  <li><strong>git status</strong> ->shows repository files added and file ready to be committed</li>
  <li><strong>git add fileNameHere</strong>-> adds a specific file to the commit queue</li>
  <li><strong>git add .</strong> -> adds all files to the queue ready to be committed</li>
  <li><strong>git commit -m "message goes here"</strong> ->committs the added files to the master.  You need to add a message otherwise there will be an error</li>
  <li><strong>git push</strong> -> merges the files and all changes with the master branch</li>
 </ul>

<h2>Branching</h2>
<p>Branching is a very usefull technique that allows us to test new features without risking damaging the master repository.  Once the feature has been tested and works as it should, it can be merged with the master. These are resources to help with branching:</p>
<ul>
  <li><a href="https://git-scm.com/book/en/v2/Git-Branching-Basic-Branching-and-Merging">Basics of Branching and Merging</a></li>
  <li><a href="https://jameschambers.co/writing/git-team-workflow-cheatsheet/">Git Team Cheatsheet</a></li>
  <li><a href="https://www.git-tower.com/learn/git/commands/git-merge">Merge command</a></li>
</ul>

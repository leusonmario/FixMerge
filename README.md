# FixMerge
 
This project is an initial prototype version of an automatic repair tool for build conflicts. The current version provides fixes for <i>Unavailable Symbol (variable and methods), Unimplemented Methods, and Duplicated Declarations</i>. Next, we provide information on how to run this tool.

## Running the tool
<ol>
 <li>
  Once the project is cloned, you must fulfill the <a href="https://github.com/leusonmario/FixMerge/blob/master/properties" target="_blank">properties</a> file with your information.
  <ul>  
     <li>
        First, you must inform your <i>login</i> and <i>password</i> of your GitHub account.
      </li>
      <li>
        The next property is <i>PathGumTree</i>, that is the location where you saved <a href="https://github.com/leusonmario/gumtree" target="_blank" >Gumtree</a>. We use an improved version of this tool, which can be found <a href="https://drive.google.com/file/d/1FUeWWiolUbPysvLjh9KyAT6COJ2-qyy5/view?usp=sharing" target="_blank" >here</a>. Download and unzip it the file. Go to the directory <i>bin</i> and inform the current local path.
      </li>
      <li>
        Next, you must inform the local path of the project. The HEAD of the project must point the commit with the broken build caused by a build conflict.
      </li>
  </ul>
 <li>
  Finally, locate the file <a href="https://github.com/leusonmario/FixMerge/blob/master/main.rb" target="_blank"><i>main.rb</i></a>, and run it by executing the command: "ruby main.rb". If the tool detects a conflict that can be fixed, it will report and ask whether you want to fix it. If yes, the tool will apply the required changes and try to compile the code. Next, it will ask you again whether you want to save the previous changes by creating a new commit.
 </li>
</ol>

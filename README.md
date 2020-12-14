# javaFX

JavaFx - the installation guide 

The instructions for this bad boy is all over the place. Sometimes, the advices and instructions are out dated or other times it just doesn't make any sense. Each IDE does something a bit differently and I present 2 straightforward options that works on a consistent basis (Linux -> Windows). 

1. Install Netbeans from this link: https://netbeans.org/community/releases/82/index.html
2. When it prompts you for which flavor, choose all.
3. Install Netbeans. Go make a celebration steak.
4. Launch Netbeans. Start working like a normal human being once again.


JavaFx - IntelliJ edition
1. Download (https://gluonhq.com/download/) 
2. Unzip the folder and place it in a directory where you'll know where to find it (Also unzip src.zip and delete it afterwards or else errors)
3. Set the global settings in IntelliJ! This can be done by the following:
  a) File -> Project Structure -> Global Libraries
  b) Click the + sign to add the damn unzipped javaFX directory.
  c) Right click on the newly added global library and click "Add to Module". Apply and OK
4. Right click on the src directory to create a new module-info.java file
5. Add the following to module-info.java in between the module's {}:
  {
    requires javafx.fxml;
    requires javafx.controls;

    opens sample;
  }
  
  Tada! It works! (On my machine at least).
  (curtesy of https://www.youtube.com/watch?v=qn2tbftFjno)

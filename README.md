## Rename multiple files or a sequence o files at once...

This shell script was created to rename several files at once that have the same base name, but are enumerated some how (in order to differentiate each one).

<hr>

### Here are some tips on how to use it:

  <br>

  ☑️ Make sure the files are inside a directory 📁 along with the script file <i>rename_multiple_siles.sh</i>
  
  <br>

  ☑️ Then, you can choose between three options to rename files, just change the value of the variable $RENAME_OPTION:
    
    ↪️ Rename files by enumerating them and keeping the same enumeration of the old files (RENAME_OPTION=1);
    
    ↪️ Rename files by enumerating them in ascending order, starting from the initial value of the variable $NUM
       with an increment as defined by the variable $NUM_INCREMENT (RENAME_OPTION=2);
    
    ↪️ Rename files by just replacing a part of the filename (RENAME_OPTION=3).
    
  <br>
  
  ☑️ Now, you need to set the extension of the files that would be renamed in the variable $FILE_EXTENSION:
  
    e.g. FILE_EXTENSION=".dat" or FILE_EXTENSION=".png"
  
  <br>
  
  ☑️ If you chose RENAME_OPTION=1 and RENAME_OPTION=2, you must define the complete name of the files,
  including the enumeration format and the file extension, in the variable $NEW_COMPLETE_NAME:
  
    e.g. NEW_COMPLETE_NAME="my_new_filename_%02d.dat"
  
  <br>
   
  ☑️ If you chose RENAME_OPTION=2, you must define the starting number and the increment of the file enumeration as previously described:
  
    e.g. NUM=1 and NUM_INCREMENT=1
    
  <br>
  
  ☑️ If you chose RENAME_OPTION=3, you must set the part of the name you want to remove in the variable $RMV_NAME, and the part you want to include in the variable $INCL_NAME:
  
    e.g. RMV_NAME="old" and INCL_NAME="new"
   
  <br>
    
  ☑️ After all, you can run the script.
  

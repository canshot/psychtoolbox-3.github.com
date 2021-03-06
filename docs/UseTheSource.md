# [UseTheSource](UseTheSource)
##### >[Psychtoolbox](Psychtoolbox)>[PsychDocumentation](PsychDocumentation)

[UseTheSource](UseTheSource) - How to access the Psychtoolbox source code.  
  
If you are interested in the source code for the C language  
modules of Psychtoolbox (i.e., the MEX file extensions  
like [Screen](Screen), [WaitSecs](WaitSecs), [GetSecs](GetSecs), [PsychHID](PsychHID), ...) then use the  
following procedure.  
  
The Psychtoolbox source code is stored in a Git code repository at  
[GitHub](GitHub).  
  
### To download the source code:  
  
1. Open a Unix terminal window on OS-X or Linux or a NT command  
   shell on M$-Windows.  
  
2. Use the "svn" commandline tool to download source code. On  
   OS-X or Linux, the svn tool is usually stored in the  
   /usr/local/bin directory, you may want to add this to your  
   PATH. On Windows, the svn client should be already in your  
   %PATH%  
  
3. The following command would download the current development branch of  
   the full PTB distribution into the subdirectory /Users/kleinerm/[MyPTB](MyPTB) :  
  
   svn checkout https://github.com/Psychtoolbox-3/Psychtoolbox-3/ /Users/kleinerm/[MyPTB](MyPTB)/  
  
   This command would download the full 'beta' distribution instead,  
   which corresponds to the most recent official, tested, production release:  
  
   svn checkout https://github.com/Psychtoolbox-3/Psychtoolbox-3/branches/beta/ /Users/kleinerm/[MyPTB](MyPTB)/  
  
   Inside the /Users/kleinerm/[MyPTB](MyPTB) folder you would see the following  
   subfolders:  
  
   Psychtoolbox/   -- The regular Psychtoolbox folder.  
   [PsychPython](PsychPython)/    -- Code for using some parts of Psychtoolbox in Python.  
   managementools/ -- Miscellaneous scripts for managing PTB releases.  
   [PsychSourceGL](PsychSourceGL)/  -- The C source code for Psychtoolbox.  
  
   Inside [PsychSourceGL](PsychSourceGL) you will find everything you need to understand  
   or to modify Psychtoolbox inner working if you are brave and patient  
   enough ;-)  
  
###    As already mentioned, the toolbox itself is split into multiple branches:  
  
   trunk  - The code that is currently under development. May or may not  
            compile and work at any given point in time, may or may not  
            be consistent. For developers and early testers only! This is  
            a view onto the [GitHub](GitHub) Git "master" branch.  
  
   beta   - Source code corresponding to the current 'beta' release, derived  
            from 'trunk'. This is what normal users should use, because  
            it is somewhat tested.  
  
   If you type the command "[PsychtoolboxVersion](PsychtoolboxVersion)" in Matlab or Octave, it  
   will tell you the flavor (trunk or beta) and SVN revision number of  
   your currently installed PTB distribution. This allows you to locate  
   the corresponding code in the GIT/SVN repository.  
  
   Be aware that you can only download code from the repository. If you  
   want to participate in PTB's development contact Mario Kleiner or  
   David Brainard for instructions. Make yourself familiar with Git if  
   you want to do serious work.  
  
   An even more recent view of current development can be found on  
   [GitHub](GitHub), where our master and experimental branches are hosted. If you  
   intend to contribute to C code development or other complex parts of  
   the software, we will require you to use git instead of Subversion and  
   you will work with the git repository at [GitHub](GitHub).  
  
   For much of the source code the MIT license applies. However, we also include  
   other 3rd party source code, libraries, [SDKs](SDKs) or tools, which are sometimes of  
   different licenses. See the file License.txt in the Psychtoolbox root folder  
   for more details. Some files contain their own license info, especially the  
   ones in the Psychtoolbox/[PsychContributed](PsychContributed) folder and [PsychSourceGL](PsychSourceGL)/Cohorts/  
   folder. If a file doesn't contain a specific license, its license may be found  
   in the Psychtoolbox/License.txt file. Otherwise it will likely be MIT licensed.  
  
   Good luck and "Use the source" (Master Yoda).  
  




<div class="code_header" style="text-align:right;">
  <span style="float:left;">Path&nbsp;&nbsp;</span> <span class="counter">Retrieve <a href=
  "https://raw.github.com/Psychtoolbox-3/Psychtoolbox-3/beta/Psychtoolbox/PsychDocumentation/UseTheSource.m">current version from GitHub</a> | View <a href=
  "https://github.com/Psychtoolbox-3/Psychtoolbox-3/commits/beta/Psychtoolbox/PsychDocumentation/UseTheSource.m">changelog</a></span>
</div>
<div class="code">
  <code>Psychtoolbox/PsychDocumentation/UseTheSource.m</code>
</div>


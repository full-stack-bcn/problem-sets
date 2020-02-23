
Git
===

1. In this exercise, we are going to play with ``git`` and its commands. 
   Describe the procedure and commands for the following:

   * Install git in your (Linux) system and set your username and e-mail.

   * In your system, create a bare repository called ``myrepo.git``.
    
   * In your system, create two clones of ``myrepo`` called ``wc1`` and ``wc2``.
    
   * In ``wc1``, create two files ``file1.txt`` and ``file2.txt`` where
      ``file1.txt`` has the content "hello" and ``file2.txt`` has the content
      "bye". Describe the command to stage your current version of
      ``file1.txt``. 
    
   * Add a line to ``file1.txt``. Which is the current state of ``file1.txt``?
    
   * Now, stage all the changes made to ``file1.txt`` and create a commit.

   * Create a conflict between ``wc1`` and ``wc2``. Describe how you know that
     there is a conflict and how you fix it.
    
   * Create a branch and commit some changes in it. Merge these changes in the
     master branch. Which type of merge is this (fast forward or 3 way merge)?
     Delete the created branch once merged.
    
    
   * Create another new branch and commit modifications in both the new branch
     and master. Merge these changes in master. Which type of merge is this
     (fast forward or 3 way merge)? Delete the branch once merged.
    
   * Create an account in [github.com](https://github.com). This account will be
     used during the course (and beyond?). From the Github control panel create
     a new empty repo and create a clone in your local system called ``wc3``.
     Use a command to see the details of the origin of ``wc3``.
    
   * Change the origin of your ``wc1`` to point to your Github repository and
     push all your changes to this Github repo.

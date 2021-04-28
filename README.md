# Password-and-Tokens-for-Jupyter-Notebook-fix-
If you upgrade Ananonda and suddenly start being prompted for password and tokens to run Jupyter Notebooks. 
I followed every thread out there and no one was clear enough on how to set this up (just 10-20 minutes max).
Follow the steps below.

 One of my problems is that I am a predominantly Linux/Ubuntu user (so hard/it doesn't come naturally navigating to the command prompt as an administrator. 'sudo' is so intuitive!). 

In Windows:

- Open Anaconda Navigator (Windows button then Run as administrator).
- Click 'Jupyter Notebook'.
- Click 'CMD.exe Prompt' (within the Navigator). Your prompt will read like 'C:\Users\User>'.
- To see a list of running instances of Jupyter Notebooks plus their tokens, type 'jupyter notebook list'.
- To set a password type 'jupyter notebook password' in the command prompt you instantiated above.
- Enter a password of your choice at the prompt 'Enter password'.
- Verify password at 'Verify password'.
- You might see '[NotebookPasswordApp] Wrote hashed password to C:\Users\User\.jupyter\jupyter_notebook_config.json'.
- To view the 'hashed' password follow the given path (above, likely in C: drive), use Notepad or VSCode (any other editor, Emacs, Nano, etc'.
- Now enter the password you created and verified earlier (first few lines above) and you are good to go (click 'login', after entering the password). 
- Important: Do not copy and paste the hashed password when prompted for password by Jupyter Notebook.
- If you get the 'incorrect password\login', shutdown all notebooks and restart Anaconda-not PC. You will be ready to work with the password protected Jupyter Notebooks until the next bug/poor (jokes!) tutorial from the developers swamping Github pages.

I hope this saves you time, inconvenience and a lot of pain! (I like to think I am of average or just below average intelligence and so need clear instructions, instead of being told to work it out myself-wastes so much time reinventing the wheel)

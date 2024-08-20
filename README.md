# injury-memos
A program that can use twitter conversations from the FPL community to update me on injuries or in the know benchings on my team. This will save me from having to scour twitter myself leading up to the deadline.

## Set-Up
1. Install the github CLI if you don't already have it (`brew install gh`).
2. Clone this repo locally. In the folder you want to clone this to, run: `gh repo clone andrewjoelpeters/injury-memos`.
3. Create a pyenv-managed virtualenv for this project in repo's root directory. Assuming you haven't executed any other commands since step 2, then `cd injury-memos` will put you in project directory.
4. Install python 3.10: `pyenv install 3.10.0`
5. Create a new virtualenv for this project called injury-memos: `pyenv virtualenv 3.10.0 injury-memos`
6. Set the virtualenv to be automatically activated for the project. Assuming you're still in the injury-memo root directory: `pyenv local injury-memos`
7. `pyenv version` should now print `injury-memos`, but if it doesn't, run `pyenv activate injury-memos` to activate the virtualenv
8. From the root directory: `pip install -r requirements.txt` to install requirements to the injury-memos virtualenv.
9. 🎉

## Making contributions
1. Make a new branch: `git checkout -b name-of-my-branch`
2. Write some code, save your changes.
3. Run `black .` to lint. This helps keep our code nicely formatted. The `.` runs black on the whole directory.
4. Use `git add`/`git commit`/`git push` to make your changes.
5. When you're ready to merge your changes to main, use `gh pr create` to create a new pull request. (I normally use the "continue in browser" option to write a description of the changes).

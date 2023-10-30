# Senier-Project

need to install : `pip3 install --upgrade ultralytics`.

PS. path is depend on your workspace.

## Train model

*not on mac M1. IT'S TRASH\
Google Colab is OK ;)

## Make Cron Job

Open terminal.

Make sure you installed `papermill` if you have anaconda `conda install -c conda-forge papermill` or `pip install papermill`.

You can check papermill path via `which papermill`.

This crontab will execution notebook everyday in 20:00 or on your depend.\
*Make sure you see [crontab](https://crontab.guru/) document for more information.

Type and open `crontab -e`.

You can use any editor that you want, such as, `vim` or `nano`.

So, The code look like this `00 20 * * * $HOME/opt/anaconda3/bin/papermill $HOME/Documents/VisualCode/Senier_Project/SenierProject.ipynb $HOME/Documents/VisualCode/Senier_Project/result.ipynb`.

After finish execution notebook, You should delete folder `/detect_img` and file `result.ipynb`.

By type this `;` followed by `rm -r $HOME/Documents/VisualCode/Senier_Project/detect_img $HOME/Documents/VisualCode/Senier_Project/result.ipynb`.

Exit, Then it's install automatic.

PS. `$HOME` and path in crontab is depend in your workspace. Recommend in full path.

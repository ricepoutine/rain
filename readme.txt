first, download:
https://fki.tic.heia-fr.ch/DBs/iamDB/data/formsA-D.tgz
https://fki.tic.heia-fr.ch/DBs/iamDB/data/formsE-H.tgz
https://fki.tic.heia-fr.ch/DBs/iamDB/data/formsI-Z.tgz
https://fki.tic.heia-fr.ch/DBs/iamDB/data/xml.tgz

then, run:
bash iam/iam.sh $IAM_USER $IAM_PASS data
where $IAM_USER and $IAM_PASS is your email and password to the IAM database

this will fail, but will create the necessary folders for the next step

then, run:
python iam/iam_par_gt.py data

this will then generate the necessary cropped images and their associated ground truths in data/pargs folders

this may take an hour

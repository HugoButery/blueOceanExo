pipeline {
  agent any
  stages {
    stage('git push') {
      steps {
        sh '''if [! \'git branch --list release\']
then git branch release
fi
git checkout release
echo "this is new content" > newfile.txt
git add *
git commit -m "a new file on new branch"
git push origin release'''
      }
    }

  }
}
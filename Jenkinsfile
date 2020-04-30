
sh 'git name-rev --name-only HEAD > GIT_BRANCH'
sh 'cat GIT_BRANCH'
git_branch = readFile('GIT_BRANCH').trim()
env.GIT_BRANCH = git_branch

stage('Deploy') {
    node {
        echo 'Pulling...' + env.BRANCH_NAME
        checkout https://github.com/nm926/prov.git

    }
}

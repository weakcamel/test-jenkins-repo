node('test') {
  stage('checkout the project') {
    checkout(
      [
        $class: 'GitSCM',
        branches: [[name: '**']],
        browser: [
          $class: 'GithubWeb',
          repoUrl: 'https://github.com/weakcamel/test-jenkins-repo'
          ],
        userRemoteConfigs: [
          [
            credentialsId: '29bdc6f0-17f1-4bfc-acaa-04a0fb18a1b1',
            url: 'https://github.com/weakcamel/test-jenkins-repo.git']
          ]
      ]
    )

  }
  stage('Build the project') {
    echo 'Building job ${env.JOB_NAME} branch ${env.BRANCH_NAME}'
  }
}

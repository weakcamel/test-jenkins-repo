echo 'llll'
checkout(
  [
    $class: 'GitSCM',
    branches: [[name: '**']],
    browser: [
      $class: 'GithubWeb',
      repoUrl: 'https://github.com/weakcamel/test-jenkins-repo'
      ],
    doGenerateSubmoduleConfigurations: false,
    extensions: [],
    submoduleCfg: [],
    userRemoteConfigs: [
      [
        credentialsId: '29bdc6f0-17f1-4bfc-acaa-04a0fb18a1b1',
        url: 'https://github.com/weakcamel/test-jenkins-repo.git']
      ]
  ]
  )

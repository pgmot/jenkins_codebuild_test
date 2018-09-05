node {
  stage('codebuild') {
    awsCodeBuild(
      projectName: 'test',
      region: 'ap-northeast-1',
      sourceControlType: 'project',
      sourceVersion: env.BRANCH_NAME,
      envVariables: "[{BRANCH_NAME,${env.BRANCH_NAME}}]",
    )
  }
}

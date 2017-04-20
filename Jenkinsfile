stage ('test') {
  //gitHubPullRequestAddComment("hello")
  pullRequest['title'] = "This title was updated by Jenkins"
  pullRequest.comment("testing 123, 456")
  pullRequest.reviewComment(pullRequest['head'], 'Jenkinsfile', 2, 'why is this commented out?')
//  for (comment in pullRequest['comments']) {
//    comment.delete()
//  }
}

stage ('test') {
  //gitHubPullRequestAddComment("hello")
  pullRequest['title'] = "This title was updated by Jenkins"
  pullRequest.comment("testing 123, 456")
  pullRequest.reviewComment(pullRequest['head'], 'Jenkinsfile', 2, 'why is this commented out?')
  pullRequest.createStatus('success', null, null, null)
  pullRequest['locked'] = !pullRequest['locked']
  
  for (assignee in pullRequest['assingees']) {
    echo assignee
  }
  
//  for (comment in pullRequest['comments']) {
//    comment.delete()
//  }
}

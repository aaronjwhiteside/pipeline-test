stage ('test') {
  //gitHubPullRequestAddComment("hello")
  pullRequest['title'] = "This title was updated by Jenkins"
//  pullRequest.comment("testing 123, 456")
//  pullRequest.reviewComment(pullRequest['head'], 'Jenkinsfile', 2, 'why is this commented out?')
  pullRequest.createStatus(status: 'success')
//  pullRequest['locked'] = !pullRequest['locked']
  
//  for (assignee in pullRequest['assignees']) {
//    echo assignee
//  }
  for (commit in pullRequest['commits']) {
    for (comment  in commit['comments']) {
      comment.replyTo('This comment was generated by Jenkins!')   
    }
  }
  
//  for (comment in pullRequest['comments']) {
//    comment.delete()
//  }
}

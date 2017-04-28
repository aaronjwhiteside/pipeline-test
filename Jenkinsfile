stage ('test') {
  //gitHubPullRequestAddComment("hello")
//  pullRequest['title'] = "This title was updated by Jenkins, testing 123"
  pullRequest['labels'] = ['bug', 'duplicate']
//  pullRequest.comment("testing 123, 456")
//  pullRequest.reviewComment(pullRequest['head'], 'Jenkinsfile', 2, 'why is this commented out?')
  pullRequest.createStatus(status: 'success')
//  pullRequest['locked'] = !pullRequest['locked']
  
//  for (assignee in pullRequest['assignees']) {
//    echo assignee
//  }
//  for (commit in pullRequest['commits']) {
//    for (comment  in commit['comments']) {
//      echo "Commit: ${commit['sha']}, Author: ${comment['user']}, Body: ${comment['body']}"
//    }
//  }
  
//  for (comment in pullRequest['comments']) {
//      echo "Comment, Author: ${comment['user']}, Body: ${comment['body']}"    
//  }
    
//  for (reviewComment in pullRequest['review_comments']) {
//      echo "Review comment, Author: ${reviewComment['user']}, Body: ${reviewComment['body']}"    
//  }    
  
//  for (comment in pullRequest['comments']) {
//    comment.delete()
//  }
}

stage ('test') {
  //gitHubPullRequestAddComment("hello")
  pullRequest['title'] = "This title was updated by Jenkins"
  pullRequest.comment("testing 123, 456")
  
  for (comment in pullRequest['comments']) {
    echo "Id: ${comment['id']}, User: ${comment['user']}, Body: ${comment['body']}, CreatedAt: ${comment['created_at']}"
  }
}
